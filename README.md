{
    "width": 50,
    "height": 1050,
    "margin": 9,
    "layer": "top",
    "position": "left",
    "spacing": 1,

    "modules-left": [
        "hyprland/workspaces",
        "clock",
        "pulseaudio",
        "cpu",
        "memory",
        "tray",
        "custom/power",
        "custom/temp"
    ],

    "modules-center": [],
    "modules-right": [],

    "hyprland/workspaces": {
        "format": "{icon}",
        "persistent-workspaces": {
            "*": 5
        },
        "format-icons": {
            "1": "1",
            "2": "2",
            "3": "3",
            "4": "4",
            "5": "5",
            "urgent": "",
            "focused": "",
            "default": ""
        }
    },

    "clock": {
        "format": "{:%H:%M}",
        "tooltip-format": "{:%Y-%m-%d}"
    },

    "custom/temp": {
        "format": "{}",
        "interval": 2,
        "exec": "/home/kerllon/.scripts/tempino.sh",
        "on-click": "psensor"
    },

    "cpu": {
        "format": "{usage}% "
    },

    "memory": {
        "format": "{}% "
    },

    "pulseaudio": {
        "format": "{volume}% {icon}",
        "format-icons": ["", "", ""],
        "on-click": "pavucontrol"
    },

    "tray": {
        "spacing": 10
    },

    "custom/power": {
        "format": "⏻",
        "on-click": "wlogout",
        "on-click-right": "systemctl poweroff",
        "on-click-middle": "systemctl reboot",
        "on-scroll-up": "brightnessctl set +5%",
        "on-scroll-down": "brightnessctl set 5%-",
        "tooltip": "Clique: Menu ╱ Direito: Desligar ╱ Meio: Reiniciar ╱ Scroll: Brilho"
    }
}
