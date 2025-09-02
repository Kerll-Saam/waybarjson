* {
font-family: "JetBrainsMono Nerd Font";
font-size: 13px;
min-height: 0;
}

window#waybar {
    background-color: rgba(200, 220, 235, 0.90);
    color: #000000;
    border-right: 2px solid rgba(135, 216, 230, 0.5);
    transition: background-color 0.5s ease;
    border-radius: 9px 9 1 5px;
    margin: 0;
    padding: 9;
}

window#waybar.hidden {
    opacity: 0.2;
}

#workspaces {
margin: 9px 0;
}

#workspaces button {
color: #6495ed;
background-color: rgba(150, 170, 237, 0.2);
border: 0.5px solid #add8e6;
padding: 6px 9;
margin: 0px 2;
border-radius: 10px;
transition: all 0.3s ease;
}

#workspaces button.active {
background-color: rgba(80, 150, 240, 0.80);
color: #0059D9;
box-shadow: 0 2px 0px rgba(255, 255, 255, 0.2);
}

#workspaces button.empty {
font-weight: bolder;
opacity: 0.6;
}

#workspaces button.urgent {
background-color: #ff4757;
color: #ffffff;
animation: pulse 2s infinite;
}

#workspaces button:hover {
background-color: rgba(150, 170, 237, 0.4);
}

#clock, #cpu, #memory, #pulseaudio, #tray, #custom-power,
#network, #battery, #backlight {
padding: 6px 6;
margin: 2.4;
}

#clock {
color: #FFEEEE;
font-weight: bold;
}

#cpu, #memory, #pulseaudio, #network, #backlight {
color: #6495ed;
}

#pulseaudio.muted {
color: #888888;
}

#tray {
color: #B8860B;
}

#battery {
color: #6495ed;
}

#battery.charging {
color: #2ed573;
}

#battery.warning:not(.charging) {
color: #ff7f50;
}

#battery.critical:not(.charging) {
color: #ff4757;
animation: blink 1s linear infinite;
}

#custom-power {
color: #ff9090;
padding: 12px 0;
background: transparent;
border: 0.2px solid #ff9595;
margin: 0.5px;
border-radius: 5px;
transition: all 0.3s ease;
}

#custom-power:hover {
background-color: rgba(0, 0, 0, 0.2);
border-color: #ff6b6b;
}

#custom-wallpaper:hover,
#pulseaudio:hover,
#cpu:hover,
#memory:hover,
#clock:hover,
#tray:hover,
#network:hover,
#battery:hover,
#backlight:hover {
background-color: rgba(170, 196, 222, 0.80);
border-radius: 5px;
}

tooltip {
    background-color: rgba(200, 220, 235, 0.95);
    border: 1px solid rgba(135, 216, 230, 0.5);
    border-radius: 5px;
}

tooltip label {
    color: #000000;
}

@keyframes pulse {
    0% { opacity: 1; }
    50% { opacity: 0.7; }
    100% { opacity: 1; }
}

@keyframes blink {
    50% { opacity: 0.5; }
}
