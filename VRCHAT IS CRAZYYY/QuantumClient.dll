using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

using MelonLoader;

using UnityEngine;

using Quantum.API.UI;
using Quantum.API.UI.QuickMenu;

namespace Quantum.Client
{
    internal static class QuantumClient
    {
        public static void Init()
        {
            InitializeClientUI();
        }

        private static void InitializeClientUI()
        {
            GameObject _buttonEmoji = UIManager.UserInterfaceGO.transform.Find("Canvas_QuickMenu(Clone)/Container/Window/QMParent/Menu_Dashboard/ScrollRect/Viewport/VerticalLayoutGroup/Buttons_QuickActions/Button_Emojis").gameObject;
            _buttonEmoji.SetActive(false);

            SubMenu _sm1 = new SubMenu("Quantum Main Menu", "QuantumMainMenu", true, UIManager.UserInterfaceGO.transform.Find("Canvas_QuickMenu(Clone)/Container/Window/QMParent/Menu_Dashboard").GetComponent<VRC.UI.Elements.Menus.LaunchPadQMMenu>());
            SubMenu _sm2 = new SubMenu("Quantum Settings", "QuantumSubMainSettings", true, UIManager.UserInterfaceGO.transform.Find("Canvas_QuickMenu(Clone)/Container/Window/QMParent/Menu_Dashboard").GetComponent<VRC.UI.Elements.Menus.LaunchPadQMMenu>());

            SimpleButton _b1 = new SimpleButton("This is a really long", "Quantum Main Menu", null, UIManager.UserInterfaceGO.transform.Find("Canvas_QuickMenu(Clone)/Container/Window/QMParent/Menu_Dashboard/ScrollRect/Viewport/VerticalLayoutGroup/Buttons_QuickActions"), new Action(() => UIManager.OpenSubMenu(UIManager.UserInterfaceGO.transform.Find("Canvas_QuickMenu(Clone)/Container/Window/QMParent/Menu_Dashboard").GetComponent<VRC.UI.Elements.Menus.LaunchPadQMMenu>(), _sm1.uiPage)));
            SimpleButton _b2 = new SimpleButton("Settings", "Quantum Settings", null, UIManager.UserInterfaceGO.transform.Find("Canvas_QuickMenu(Clone)/Container/Window/QMParent/Menu_QuantumMainMenu/ScrollRect/Viewport/VerticalLayoutGroup"), new Action(() => UIManager.OpenSubMenu(UIManager.UserInterfaceGO.transform.Find("Canvas_QuickMenu(Clone)/Container/Window/QMParent/Menu_Dashboard").GetComponent<VRC.UI.Elements.Menus.LaunchPadQMMenu>(), _sm2.uiPage)));
            SimpleButton _b3 = new SimpleButton("u gae", "u big gae", null, UIManager.UserInterfaceGO.transform.Find("Canvas_QuickMenu(Clone)/Container/Window/QMParent/Menu_QuantumMainMenu/ScrollRect/Viewport/VerticalLayoutGroup"), new Action(() => QMain.Instance.LoggerInstance.Msg("why u so gae")));
            SimpleButton _b4 = new SimpleButton("another button", "idk anymore", null, UIManager.UserInterfaceGO.transform.Find("Canvas_QuickMenu(Clone)/Container/Window/QMParent/Menu_QuantumSubMainSettings/ScrollRect/Viewport/VerticalLayoutGroup"), new Action(() => QMain.Instance.LoggerInstance.Msg("i really don't know")));
        }
    }
}
