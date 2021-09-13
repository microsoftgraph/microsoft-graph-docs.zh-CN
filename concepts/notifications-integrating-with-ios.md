---
title: 将 iOS 应用与用户通知客户端 SDK 相集成
description: 将 iOS 应用与用户通知客户端 SDK 相集成。
ms.localizationpriority: high
ms.prod: notifications
ms.openlocfilehash: 0a73626317195320a274430f32607f13b9920505
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59066931"
---
# <a name="integrate-your-ios-app-with-the-client-side-sdk-for-user-notifications"></a>将 iOS 应用与用户通知客户端 SDK 相集成

在 Azure 门户[注册你的应用](notifications-integration-app-registration.md)并在合作伙伴开发人员中心载入你的[跨设备体验](notifications-integration-cross-device-experiences-onboarding.md)之后，下一步是将客户端应用与适用于 iOS 应用的客户端 SDK 相集成。  

借助客户端 SDK，你的应用可以执行所需的注册步骤，以开始接收从应用服务器发布的面向当前登录用户的通知。 SDK 随后会管理客户端上的通知，包括接收新传入的通知，管理通知状态以实现全局消除等方案，以及检索完整的通知历史记录。 

## <a name="new-incoming-notification-flow"></a>新传入的通知流

对于接收新传入的通知，数据流如下图所示。

![iOS 应用的新通知流](images/notifications-new-notification-ios.png)

该过程涉及几个组件：

* 应用服务器 - 应用程序的后端
* 应用客户端 - 应用程序的前端（UWP 应用、Android 应用或 iOS 应用）
* Microsoft Graph 通知 - 一种服务组件，支持在跨设备和平台的各种应用客户端实例中发布、存储和同步用户通知
* APN - Apple 为 iOS 应用提供的 Apple 推送通知服务。 Microsoft Graph 通知使用此服务向 iOS 应用客户端发送有关用户通知数据更改的信号。  

该图显示了以下步骤： 

1. 应用逻辑。这一步抓住了触发通知发布给用户的因素。这是特定于应用的逻辑，它可以是 Microsoft Graph 中的事件或其他内容的数据更新（例如新的日历事件或任务分配），也可以是应用服务希望向用户通知的其他内容。
2. 应用服务器通过 Microsoft Graph 通知 API 向目标用户发布通知。 有关详细信息，请参阅[服务器端集成](notifications-integrating-app-server.md)。
3. 在收到包含新通知的 Web 请求后，Microsoft Graph 通知会在此应用和此用户的云中安全地保留通知内容。
4. 对于订阅接收此用户通知的每个应用客户端实例，Microsoft Graph 通知会通过操作系统提供的本机推送服务发送信号以通知应用客户端。 在这种情况下，应用程序是 iOS 应用，它使用[APN 后台更新通知]来发送信号。 
5. 由传入的推送通知向应用程序发出信号后，它会要求 SDK 获取用户通知存储区中的更改。 
6. SDK 将与 Microsoft Graph 中的用户通知存储区建立安全且合规的连接。
7. SDK 将获取数据更改 - 在本例中为新通知内容。 
8. SDK 会触发事件回调，以在成功检索到更改后通知该应用。 
9. 应用程序逻辑。 此步骤可捕获你的应用选择在事件回调内执行的操作。 通常，这会导致本地应用数据更改和本地 UI 更新。 在这种情况下，该应用通常会构建 iOS 警报以通知用户有关通知内容的信息。

## <a name="notification-update-flow"></a>更新通知流

使用 Microsoft Graph 通知的主要好处之一是它可以安全地在云中保留通知，并将其转换为有状态资源类型。 因此，它可以帮助你的应用在跨设备方案中为同一登录用户跨不同设备管理和同步通知的正确状态。 当某台设备上的通知已标记为“已消除”或“已读”时，可以实时通知其他设备。 作为用户通知体验的一部分，可以真正实现“处理一次，每处均消除”的效果。 

下图显示了在一台设备上更改通知状态或删除通知，以及在另一台设备上接收/处理状态更改或删除的数据流。

![iOS 应用的更新通知流](images/notifications-notification-update-ios.png)

请注意，流程的第二部分与处理新传入通知的流程类似。这是设计使然 - 设计的 SDK 编程模式使应用程序客户端可以相似的方式处理所有类型的用户通知数据更改 (新传入的通知、通知状态更改、已删除的通知)。  

该图显示了以下步骤：

1. 应用程序逻辑。 某事件触发了要更改或删除的通知。 一般来说，任何事件均可触发更改通知。 
2. 调用客户端 SDK 以更新或删除通知的应用。 目前，我们公布了两种与状态更改相关的属性 - **userActionState** 和 **readState**，但是，应用程序可以定义这些状态以及何时需要更新它们。 例如，当用户消除通知弹出窗口时，你可以将 **userActionState** 更新为“已消除”。 当用户单击通知弹出窗口并启动应用以使用相应的应用内容时，你可以将 **userActionState** 更新为“已激活”和并将 **readState** 更新为“已读”。 
3. 调用相应的 API 以更新或删除通知后，SDK 将调用云中的用户通知存储区，以将此更改扇出至同一登录用户的其他应用客户端实例。 
4. 从客户端接收更新/删除请求时，Microsoft Graph 通知将更新通知存储区，并标识已订阅此更改的其他应用客户端实例。
5. 对于每个应用客户端订阅，Microsoft Graph 通知会通过操作系统提供的本机推送服务发送信号以通知应用客户端。 在这种情况下，它是 iOS 应用，并使用 [APN 后台更新通知](https://developer.apple.com/library/archive/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/CreatingtheNotificationPayload.html#//apple_ref/doc/uid/TP40008194-CH10-SW8)来发送信号。 
6. 由传入的推送通知向应用程序发出信号后，它会要求 SDK 获取用户通知存储区中的更改。 
7. SDK 将与 Microsoft Graph 中的用户通知存储区建立安全且合规的连接。
8. SDK 获取数据更改 - 在这种情况下，更改为通知状态更新或通知删除。 
9. SDK 会触发事件回调，以在成功检索到更改后通知该应用。 
10. 应用程序逻辑。 此步骤可捕获你的应用选择在事件回调内执行的操作。 通常，这会导致本地应用数据更改和本地 UI 更新。 在这种情况下，由于存在通知更新，因此应用应本地更新 UI 以反映状态更改。 例如，如果通知已标记为“已激活”，则你可以删除 iOS 通知中心内的相应警报 UI，以实现“处理一次，每处均消除”的效果。 

有关 Microsoft Graph 通知的详细信息，请参阅 [Microsoft Graph 通知概述](notifications-concept-overview.md)。 与 Microsoft Graph 通知进行端到端集成所需步骤相关的详细信息，请参阅 Microsoft Graph 通知[集成概述](notifications-integration-e2e-overview.md)。

## <a name="adding-the-sdk-to-your-project"></a>向项目添加 SDK

将连接设备平台添加到 iOS 应用的最简单方法是使用 [CocoaPods](https://cocoapods.org/) 依存关系管理器。 转到 iOS 项目的 *Podfile* 并插入以下条目：

```ObjectiveC
platform :ios, "10.0"
workspace 'iOSSample'

target 'iOSSample' do
  # Uncomment the next line if you're using Swift or would like to use dynamic frameworks
  # use_frameworks!

    pod 'ProjectRomeSdk'

  # Pods for iOSSample
```

> [!NOTE]
> 若要使用 CocoaPod，你必须在项目中使用 _.xcworkspace_ 文件。

## <a name="initializing-the-connected-device-platforms"></a>初始化连接设备平台

客户端 SDK 构建在称为“连接设备平台”的基础结构之上。 在使用任何功能之前，必须在你的应用中初始化该平台。 应该通过 **AppDelegate** 方法执行初始化步骤，因为在通知方案发生之前必须执行这些步骤。

你必须通过实例化 [**MCDConnectedDevicesPlatform**](/windows/project-rome/objectivec-api/connecteddevices/mcdconnecteddevicesplatform) 类来构建并初始化该平台。 在执行此操作之前，请确保挂接事件处理程序，如图所示，因为在启动平台后，事件可能会开始触发。  

```ObjectiveC
MCDConnectedDevicesPlatform* platform = [MCDConnectedDevicesPlatform new];
        
[platform.accountManager.accessTokenRequested subscribe:^(MCDConnectedDevicesAccountManager* _Nonnull manager, MCDConnectedDevicesAccessTokenRequestedEventArgs* _Nonnull args) {
    // implement the callback;
}];
        
[self.platform.accountManager.accessTokenInvalidated
    subscribe:^(MCDConnectedDevicesAccountManager* _Nonnull manager __unused,
        MCDConnectedDevicesAccessTokenInvalidatedEventArgs* _Nonnull request) {
    // implement the callback;
}];
        
[self.platform.notificationRegistrationManager.notificationRegistrationStateChanged subscribe:^(MCDConnectedDevicesNotificationRegistrationManager* _Nonnull manager __unused, MCDConnectedDevicesNotificationRegistrationStateChangedEventArgs* _Nonnull args) {
    // implement the callback
}];
        
[platform start];
```

### <a name="handling-account-access-token"></a>处理帐户访问令牌

SDK 发起的所有 Web 调用（包括检索新传入通知的内容、更新通知状态等）都会读取或写入用户的数据，因此始终需要有效的访问令牌。 SDK 要求你处理以下事件 - 在请求访问令牌或访问令牌失效时调用 - 以确保在初始化平台后正确处理用户的访问令牌。 

#### <a name="accesstokenrequested"></a>accessTokenRequested

有关完整实施，请参阅 [iOS 示例应用](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m)。 

#### <a name="accesstokeninvalidated"></a>accessTokenInvalidated

有关完整实施，请参阅 [iOS 示例应用](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m)。 

```ObjectiveC
[platform.accountManager.accessTokenInvalidated
    subscribe:^(MCDConnectedDevicesAccountManager* _Nonnull manager __unused,
        MCDConnectedDevicesAccessTokenInvalidatedEventArgs* _Nonnull request) {
}];
```

### <a name="handling-push-registration-expiration"></a>处理推送注册过期 

Microsoft Graph 通知使用 APN（iOS 上的本机推送平台）向客户端应用程序发送有关用户通知数据更改的信号。 当从应用服务器发布新传入的通知时，或者在跨设备方案中的具有同一登录用户的其他设备上更新任何通知状态时，会发生这种情况。 

因此，需要一个允许后台更新通知成功通过的有效 APN 令牌。 以下事件回调负责处理 APN 推送令牌过期。 

#### <a name="notificationregistrationstatechanged"></a>notificationRegistrationStateChanged

有关完整实施，请参阅 [iOS 示例应用](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m)。 

## <a name="signing-in-your-user"></a>登录用户

与 Microsoft Graph 中的许多其他资源类型一样，Microsoft Graph 通知也以用户为中心。 为了让你的应用订阅并开始接收已登录用户的通知，你首先需要获取在注册过程中使用的有效 OAuth 令牌。 你可以使用生成和管理 OAuth 令牌的首选方法。 示例应用使用 ADAL。 

如果你使用的是 Microsoft 帐户，则需要在登录请求中包含以下权限：`wl.offline_access"`、`ccs.ReadWrite`、`wns.connect`、`asimovrome.telemetry` 和 `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`。 

如果你使用的是 Azure AD 帐户，则需要请求以下受众：`https://cdpcs.access.microsoft.com`。

## <a name="adding-the-user-account-to-the-platform"></a>将用户帐户添加到平台 

你需要使用 SDK 注册已登录用户的帐户。 这涉及添加帐户并注册推送通道以通过 APN 接收初始推送通知。 有关详细信息，请参阅示例中的 [prepareAccountAsync](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m) 方法。

```ObjectiveC
MCDConnectedDevicesPlatform* platform = [MCDConnectedDevicesPlatform new];
MCDConnectedDevicesAccount* mcdAccount = [MCDConnectedDevicesAccount new];

[platform.accountManager addAccountAsync:mcdAccount callback:adapter]; 
```

## <a name="subscribing-to-receive-users-notifications"></a>订阅以接收用户的通知 

你需要为此已登录用户实例化应用程序的 **UserDataFeed** 对象。 你的应用程序由你在[跨设备体验载入](notifications-integration-cross-device-experiences-onboarding.md)过程中提供的跨平台应用 ID 进行标识。

```ObjectiveC
// Initialize the feed and subscribe for notifications
MCDUserDataFeed* feed = [MCDUserDataFeed getForAccount:account
                        platform:platform
                        activitySourceHost:APP_HOST_NAME];

NSArray<MCDUserDataFeedSyncScope*>* syncScopes = @[ [MCDUserNotificationChannel syncScope] ];
[feed subscribeToSyncScopesAsync:syncScopes
        callback:^(BOOL success __unused, NSError* _Nullable error __unused) {
    // Start syncing down notifications
    [feed startSync];
}];
```

## <a name="receiving-and-managing-user-notifications"></a>接收和管理用户通知

本主题前面的流程图显示，处理来自应用服务器的新传入通知的编程模式与处理从另一个应用客户端实例启动的通知更新或删除的编程模式类似。以下是处理这些数据更改的步骤。 

### <a name="handling-incoming-push-notification-signal"></a>处理传入推送通知信号

所有类型的用户通知数据更改均会生成一个作为推送通知传递至应用客户端的信号。 对于 iOS 应用，信号将作为 APN 后台更新通知进行传送。 接收数据消息信号时，应用应调用 **TryParse** 以触发 SDK 从 Microsoft Graph 通知服务中提取实际数据更改。

```ObjectiveC
// App running in background and received a push notification, launched by user tapping the alert view
MCDConnectedDevicesNotification* notification = [MCDConnectedDevicesNotification tryParse:notificationInfo];
if (notification != nil) {
    [_platformManager.platform processNotificationAsync:notification
            completion:^(NSError* error __unused) {
        // NOTE: it may be useful to attach completion to this async in order to know when the
        // notification is done being processed.
        // This would be a good time to stop a background service or otherwise cleanup.
    }];
} else {
    NSLog(@"Remote notification is not for ConnectedDevicesPlatform, skip processing");
}
```

### <a name="handling-user-notification-data-changes"></a>处理用户通知数据更改

SDK 成功提取数据更改之后，将会调用事件回调且应用客户端有望处理通知创建、更新或删除。

```ObjectiveC
[reader readBatchAsyncWithMaxSize:100 completion:^(NSArray<MCDUserNotification *> * _Nullable notifications,
                                                    NSError * _Nullable error) {
    if (error) {
    } else {
        for (MCDUserNotification* notification in self.notifications) {
        // Handle notification change based on change type;
        }
        }
    }
}];
```

### <a name="update-state-of-a-notification"></a>更新通知状态

如果从此应用客户端实例发起通知状态更改（例如，如果此设备上的定制通知弹出窗口由用户激活），则应用需要调用 SDK 更新通知状态，以便在同一用户使用的所有设备中同步此状态更改操作。 

```ObjectiveC
- (void)dismissNotification:(MCDUserNotification*)notification {
    if (notification.userActionState == MCDUserNotificationUserActionStateNoInteraction) {
        [self dismissNotificationFromTrayWithId:notification.notificationId];
        notification.userActionState = MCDUserNotificationUserActionStateDismissed;
        [notification saveAsync:^(__unused MCDUserNotificationUpdateResult * _Nullable result, __unused NSError * _Nullable error) {
        // handle result;
         }];
    }
}
```

### <a name="delete-a-notifications"></a>删除通知

如果从此应用客户端实例发起通知删除（例如，如果此通知对应的任务标记为“完成”并从应用数据库中删除），则应用需要调用 SDK 删除通知，以便在同一用户使用的所有设备中同步此删除操作。 

仅当通知过期或者被显式删除时，它才会从用户通知存储区中删除。 将 **UserActionState** 更新为“已消除”时，用户通知不会删除，因为 **UserActionState** 的语义定义是由应用程序本身定义。

```Obj-C
- (void)deleteNotification:(MCDUserNotification*)notification {
    [_channel deleteUserNotificationAsync:notification.notificationId
     completion:^(__unused MCDUserNotificationUpdateResult* _Nullable result, NSError* _Nullable error) {
        // handle result;
     }];
}
```

## <a name="see-also"></a>另请参阅

- [API 参考](/windows/project-rome/notifications/api-reference-for-ios/)，以获取与 SDK 中的通知功能相关的整套 API。 
- 适用于 Android 应用的[客户端示例](https://github.com/Microsoft/project-rome/tree/master/iOS/samples/GraphNotifications)。
- 适合于发布通知的[应用服务器示例](notifications-integrating-app-server.md)。
