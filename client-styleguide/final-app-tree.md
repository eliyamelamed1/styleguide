# Analytical App Structure

```plaintext
final-app/
├── components/
│   ├── (UI)/
│   │   │── Button
│   │   │   ├── Button.jsx
│   │   │   └── Button.less
│   │   │── InputField
│   │   │   ├── InputField.jsx
│   │   │   └── InputField.less
│   │   │── Modal
│   │   │   ├── Modal.jsx
│   │   │   └── Modal.less
│   │   │── Avatar
│   │   │   ├── Avatar.jsx
│   │   │   └── Avatar.less
│   │   │── Tooltip
│   │   │   ├── Tooltip.jsx
│   │   │   └── Tooltip.less
│   │   │── DropdownMenu
│   │   │   ├── DropdownMenu.jsx
│   │   │   └── DropdownMenu.less
│   ├── Navbar.jsx
│   └── SideMenu.jsx
│
├── hooks/
│   ├── useFetch.js
│   ├── useBool.js
│   ├── useAnimation.js
│   └── useForceState.js
│
├── features/
│   ├── SearchBar/
│   │   ├── components/
│   │   │   ├── SearchBar/
│   │   │   │   ├── SearchBar.jsx
│   │   │   │   └── SearchBar.less
│   │   │   ├── SearchBarComponent/
│   │   │   │   ├── SearchBarComponent.jsx
│   │   │   │   └── SearchBarComponent.less
│   │   │   └── FilterComponent/
│   │   │   │   └── FilterComponent.jsx
│   │   │   │   └── FilterComponent.less
│   │   ├── hooks/
│   │   │   ├── useSearchQuery.js
│   │   │   └── useSearchResults.js
│   │   ├── utils/
│   │   │   ├── searchHelpers.js
│   │   │   └── filterHelpers.js
│   │   └── index.js
│   ├── Messaging/
│   │   ├── components/
│   │   │   ├── MessageListComponent/
│   │   │   │   ├── MessageListComponent.jsx
│   │   │   │   └── MessageListComponent.less
│   │   │   └── MessageItemComponent/
│   │   │   │   └── MessageItemComponent.jsx
│   │   │   │   └── MessageItemComponent.less
│   │   ├── hooks/
│   │   │   ├── useMessages.js
│   │   │   └── useNewMessageNotification.js
│   │   ├── utils/
│   │   │   ├── messageFormatter.js
│   │   │   └── messageSorter.js
│   │   └── index.js
│   └── Notifications/
│       ├── components/
│       │   ├── NotificationListComponent/
│       │   │   ├── NotificationListComponent.jsx
│       │   │   └── NotificationListComponent.less
│       │   └── NotificationItemComponent/
│       │   │   ├── NotificationItemComponent.jsx
│       │   │   └── NotificationItemComponent.less
│       ├── hooks/
│       │   ├── useNotifications.js
│       │   └── useNotificationSettings.js
│       ├── utils/
│       │   ├── notificationHelpers.js
│       │   └── notificationFormatter.js
│       └── index.js
│
├── pages/
│   ├── HomePage/
│   │   ├── HomePage.jsx
│   │   └── HomePage.less
│   └── ResearchPage/
│       ├── ResearchPage.jsx
│       ├── ResearchPage.less
│       └── features/
│           ├── Dashboards/
│           │   ├── components/
│           │   │   ├── DashboardComponent/
│           │   │   │   ├── DashboardComponent.jsx
│           │   │   │   └──DashboardComponent.less
│           │   │   ├── WidgetComponent/
│           │   │   │   ├── WidgetComponent.jsx
│           │   │   │   └── WidgetComponent.less
│           │   ├── hooks/
│           │   │   ├── useDashboardData.js
│           │   │   └── useWidgetSettings.js
│           │   ├── utils/
│           │   │   ├── dashboardHelpers.js
│           │   │   └── widgetHelpers.js
│           │   └── index.js
│           └── Insights/
│               ├── components/
│               │   ├── InsightsComponent/
│               │   │   ├── InsightsComponent.jsx
│               │   │   └── InsightsComponent.less
│               │   ├── InsightsGraphComponent/
│               │   │   ├── InsightsGraphComponent.jsx
│               │   │   └── InsightsGraphComponent.less
│               ├── hooks/
│               │   ├── useInsightsData.js
│               │   └── useInsightsAnalysis.js
│               ├── utils/
│               │   ├── insightsHelpers.js
│               │   └── insightsFormatter.js
│               └── index.js
