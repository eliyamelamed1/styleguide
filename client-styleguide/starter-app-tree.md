# Analytical App Structure

```plaintext
starter-app/
├── components/
│   ├── DashboardComponent/
│   │   ├── DashboardComponent.jsx
│   │   └── DashboardComponent.less
│   ├── WidgetComponent/
│   │   ├── WidgetComponent.jsx
│   │   └── WidgetComponent.less
│   ├── MessageListComponent/
│   │   ├── MessageListComponent.jsx
│   │   └── MessageListComponent.less
│   ├── MessageItemComponent/
│   │   ├── MessageItemComponent.jsx
│   │   └── MessageItemComponent.less
│   ├── InsightsComponent/
│   │   ├── InsightsComponent.jsx
│   │   └── InsightsComponent.less
│   ├── InsightsGraphComponent/
│   │   ├── InsightsGraphComponent.jsx
│   │   └── InsightsGraphComponent.less
│   ├── NotificationListComponent/
│   │   ├── NotificationListComponent.jsx
│   │   └── NotificationListComponent.less
│   ├── NotificationItemComponent/
│   │   ├── NotificationItemComponent.jsx
│   │   └── NotificationItemComponent.less
│   ├── Button/
│   │   ├── Button.jsx
│   │   └── Button.less
│   ├── InputField/
│   │   ├── InputField.jsx
│   │   └── InputField.less
│   ├── Modal/
│   │   ├── Modal.jsx
│   │   └── Modal.less
│   ├── Avatar/
│   │   ├── Avatar.jsx
│   │   └── Avatar.less
│   ├── Tooltip/
│   │   ├── Tooltip.jsx
│   │   └── Tooltip.less
│   ├── DropdownMenu/
│   │   ├── DropdownMenu.jsx
│   │   └── DropdownMenu.less
│   ├── Navbar/
│   │   ├── Navbar.jsx
│   │   └── Navbar.less
│   ├── SearchBar/
│   │   ├── SearchBar.jsx
│   │   └── SearchBar.less
│   ├── SideMenu/
│   │   ├── SideMenu.jsx
│   │   └── SideMenu.less
│   ├── SearchBarComponent/
│   │   ├── SearchBarComponent.jsx
│   │   └── SearchBarComponent.less
│   └── FilterComponent/
│       ├── FilterComponent.jsx
│       └── FilterComponent.less
│
├── hooks/
│   ├── useDashboardData.js
│   ├── useWidgetSettings.js
│   ├── useMessages.js
│   ├── useNewMessageNotification.js
│   ├── useInsightsData.js
│   ├── useInsightsAnalysis.js
│   ├── useNotifications.js
│   ├── useNotificationSettings.js
│   ├── useFetch.js
│   ├── useBool.js
│   ├── useAnimation.js
│   ├── useForceState.js
│   ├── useSearchQuery.js
│   └── useSearchResults.js
│
├── utils/
│   ├── messageFormatter.js
│   ├── messageSorter.js
│   ├── insightsHelpers.js
│   ├── insightsFormatter.js
│   ├── dashboardHelpers.js
│   ├── widgetHelpers.js
│   ├── notificationHelpers.js
│   ├── notificationFormatter.js
│   ├── searchHelpers.js
│   └── filterHelpers.js
│
└── pages/
    ├── HomePage/
    │   ├── HomePage.jsx
    │   └── HomePage.less
    └── ResearchPage/
        ├── ResearchPage.jsx
        └── ResearchPage.less
