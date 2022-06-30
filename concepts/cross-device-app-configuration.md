---
title: '构建由 Project Rome 提供支持的跨设备应用 '
description: 使用活动源和设备中继 API 无缝地构建跨设备和平台的体验，以减少用户的摩擦并推动应用使用。
ms.localizationpriority: medium
ms.prod: project-rome
ms.openlocfilehash: 0c4738b39eeb88b52a5a6d0d43f3f15103f76b7b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440941"
---
# <a name="build-cross-device-apps-powered-by-project-rome"></a>构建由 Project Rome 提供支持的跨设备应用

可以使用 Project Rome 构建无缝跨设备和平台的体验，从而为用户减少摩擦并帮助促进应用参与。 对于要使用 Project Rome API 跨设备和平台共享数据的应用程序，你需要配置跨设备应用，其中包含有关你特定于平台的应用的信息。 

跨设备应用使你能够： 

- 使用 Microsoft Graph 中的 Project Rome 活动源 API。  
- 使用适用于 Windows、Android 和/或 iOS 的 Project Rome SDK 读取和写入由一组特定于平台的应用程序发布的用户活动。
- 使用适用于 Android 或 iOS 的 Project Rome SDK 通过 Project Rome 中的设备中继功能定位应用。

**使用活动源 API 跨设备从中断的位置继续**

可以将跨设备应用配置为关联适用于 Windows、iOS、Android、Web 的应用，以便每个平台上的应用都可以读取和写入由组中任意应用发布的用户活动。 

例如，在与朋友共进晚餐之前，用户在她的 PC 上撰写新闻稿。 在餐厅，她收到来自老板的通知，需要尽快修改一个输入错误。 她在她的 Android 手机上打开应用并看到显示早期编辑的新闻稿的卡片。 她点击该卡片将其打开，以便可以立即修改新闻稿并回到她的朋友身边。 
 
此跨设备应用配置就绪后，毫不费力地跨设备和平台同步用户的活动源，以便可以构建帮助用户在任何应用平台上中断的位置继续执行重要任务的体验。 

**使用设备中继 API 在正确的时间选择正确的屏幕**

可以使用推送通知凭据为你的应用可用的每个平台配置跨设备应用，以便可以在使用应用的任何设备（无论何种平台）上将命令或通知传递给你。 

例如，用户在下班回家的公交车上观看视频。 当她回到家时，她点击应用在她的 Xbox One 上启动视频，则可以继续在大屏幕上观看。 

将你的应用可用的每个平台的推送通知凭据与跨设备应用关联时，用户的应用可以跨设备发送命令，以便可以构建跨多个屏幕的体验或实时将工作流从一个设备转换到另一个设备的体验。 

## <a name="select-the-right-hosting-method-for-your-cross-device-app-configuration"></a>为跨设备应用配置选择正确的托管方法
可以将跨设备应用配置作为域上的 JSON 文件或作为可通过 [Windows 开发人员中心](https://developer.microsoft.com/windows)配置的配置文件进行托管。 根据要在应用中启用的 Project Rome 功能选择托管选项。 

### <a name="windows-dev-center-profile-recommended"></a>Windows 开发人员中心配置文件（推荐） 
可以使用 [Windows 开发人员中心](https://developer.microsoft.com/windows)中管理的跨设备应用访问所有 Project Rome 功能。 Windows 开发人员中心还提供管理任何跨设备应用配置更改的 *最佳* 方式。 可以更安全地将更新保存到现有配置文件，直到已准备好将更改发布到生产中。 将更改发布到开发人员中心中的现有跨设备应用时，新配置文件将在大约 **1 小时** 后生效。  

### <a name="externally-hosted-json-file-limited"></a>外部托管的 JSON 文件（有限） 
可以通过作为外部托管的 JSON 文件管理的跨设备应用在所有受支持的平台上使用以下 Project Rome 功能：  

* 使用[活动源 API](/graph/api/resources/activity-feed-api-overview) 读取和写入所有平台中的用户活动
* 使用 Project Rome SDK 写入所有平台（Windows、iOS、Android、Web）中的用户活动。

如果 **仅** 访问这些功能，则可以将跨设备应用配置作为域上的 JSON 文件进行外部托管。

## <a name="configure-a-cross-device-app-using-the-windows-dev-center"></a>使用 Windows 开发人员中心配置跨设备应用
跨设备应用 ID 表示为你拥有的域。 域指向作为域上托管的 JSON 文件存储或可通过 Windows 开发人员中心配置的特定于平台的应用 ID 的映射。 确定将用来表示跨设备应用 ID 的域后，将需要收集信息来配置关联的配置文件。 

### <a name="step-1-select-a-secure-domain-for-your-cross-device-app-id-and-enable-domain-verification"></a>步骤 1：为跨设备应用 ID 选择安全域并启用域验证
用作跨设备应用 ID 的域必须为顶级域或子域，且必须通过 TLS 保护。 例如：https://contoso.com 或 https://myapp.contoso.com，但不是 https://myapp.contoso.com/somepath。 **每个跨设备应用必须具有唯一域（或子域）。** 但是，根据要支持的跨平台行为决定将哪些应用与单个跨设备应用关联。 

例如，具有一套游戏应用的应用开发人员可能会对每个游戏应用使用单独的子域，以确保每个应用仅在跨设备和平台读取数据时可以继续执行的用户活动中订阅。 另一方面，具有一套旨在协同工作的效率类应用的应用开发人员可能会对所有这些效率类应用使用单个域，以便应用能够跨设备启动该套件的成员。  

#### <a name="assert-domain-ownership-with-the-windows-dev-center"></a>通过 Windows 开发人员中心声明域所有权
使用 Windows 开发人员中心管理跨设备应用配置时，表示跨设备应用 ID 的域会作为跨设备应用配置文件的一部分进行存储，因此 Microsoft 可以确认你是域所有者。 要完成跨设备应用配置的发布，**必须验证** 你的域所有权，因此最好先处理此事。 如果尚未验证域，则可以保存跨设备应用详细信息并在完成此步骤后重新运行验证，以便可以发布跨设备应用。

若要声明跨设备应用的域所有权，将需要为域添加具有在开发人员中心中为你提供的唯一值的 [DNS TXT](https://go.microsoft.com/fwlink/?linkid=871417) 条目。 每个跨设备应用的此值都是唯一的。 若要查找应用的唯一值，请登录到 Windows 开发人员中心，然后从左侧菜单中选择“跨设备体验”以开始配置新的跨设备应用。 为新的跨设备应用提供名称后，从子菜单中选择“验证跨设备应用域”。 此页将显示具有唯一内 **联** 值的说明 (例如，MS=95ff4557-813f-45a5-b2f6-1f94170b979f) 。 确保复制整个值，包括“MS=”。

### <a name="step-2-collect-your-platform-specific-application-ids"></a>步骤 2：收集特定于平台的应用程序 ID
为将使用 [Project Rome API](/graph/api/resources/project-rome-overview) 的每个应用程序和平台收集特定于平台的应用程序 ID。

将需要收集每个特定于平台的应用程序 ID，才能将其与跨设备应用标识关联。 使用 Windows 开发人员中心，将能够从与开发人员帐户关联的通用 Windows 平台应用中进行选择，但需要手动提供任何 win32、iOS 或 Android 应用的应用程序 ID 并标识任何关联 Web 应用的主 URL。 每个平台最多可以关联 10 个 ID。 

若要查找 ID，请执行以下操作：

* **windows_universal** - 为每个 UWP 应用提供 AUMID。 有关详细信息，请参阅[查找已安装应用 (Industry 8.1) 的应用程序用户模型 ID](/previous-versions/windows/embedded/dn449300(v=winembedded.82)) 和[应用程序](/uwp/schemas/appxpackage/appxmanifestschema/element-application)。
* **windows_win32** - 为每个应用提供 AUMID。 对于 win32 应用，将需要使用脚本来检索此信息。 有关详细信息，请参阅[查找已安装应用 (Industry 8.1) 的应用程序用户模型 ID](/previous-versions/windows/embedded/dn449300(v=winembedded.82))。
* **android** - 有关详细信息，请参阅 [更改包名称](https://developer.android.com/studio/build/application-id.html#change_the_package_name)。 
* **ios** - 有关详细信息，请参阅 [捆绑](https://developer.apple.com/documentation/foundation/bundle)和 [必需、可本地化和可编辑属性](https://help.apple.com/itunes-connect/developer/#/devfc3066644)。
* **msa** – 登录到 [应用程序注册门户](https://apps.dev.microsoft.com)。 可以查看任何应用的应用 ID/客户端 ID。 同时支持 Live SDK（十六进制值）和聚合应用 ID (GUID)。   

### <a name="step-3-configure-support-for-microsoft-account-or-azure-ad"></a>步骤 3：配置对 Microsoft 帐户或 Azure AD 的支持
若要启用跨设备体验，应用用户必须使用 [Microsoft 帐户](https://account.microsoft.com/account) 或 [Azure Active Directory (Azure](/azure/active-directory/develop/active-directory-developers-guide) AD) 帐户登录。 你将提供应用 ID/客户端 ID 以在跨设备应用配置过程中支持身份验证，从而启用跨平台支持。 最多可提供 10 个实例。

可以通过使用你的开发人员帐户登录到[应用程序注册门户](https://apps.dev.microsoft.com)来查找现有应用 ID/客户端 ID 或预配新应用 ID/客户端 ID。 登录到门户后，可以查看任何应用的应用 ID/客户端 ID。 同时支持 Live SDK（十六进制值）和聚合应用 ID (GUID)。   

如果正在构建将支持 Azure AD 用户的应用程序，且不使用通过[应用程序注册门户](https://apps.dev.microsoft.com)颁发的聚合应用程序 ID，则将需要为 Azure 应用的应用程序 ID 提供 GUID。 若要查找租户的 GUID，请执行以下操作： 

1. 登录到 [Azure 门户](https://portal.azure.com)。 
2. 选择“Azure Active Directory”。
3. 在“管理”下，选择“应用注册”。 
4. 从列表中选择你的应用并查看“概要”下列出的应用程序 ID (GUID)。

### <a name="step-4-configure-support-for-cross-platform-push-notifications-optional"></a>步骤 4：配置对跨平台推送通知的支持（可选） 
如果已选择在 Windows 开发人员中心中配置跨设备应用，则可以通过为 Android 和 iOS 推送消息平台提供用于 API 的凭据来启用对跨平台推送通知的支持。 如果使用适用于 iOS 和 Android 的 Project Rome SDK 且希望完成的不止是发布用户活动，则需要执行以上步骤。 如果仅使用适用于 Microsoft Graph 的 Project Rome API，则无需执行此步骤。 每个平台最多可以关联 10 组凭据。 

> [!IMPORTANT]
> 不要将推送通知凭据存储在外部托管的 JSON 文件中。

若要查找 ID，请执行以下操作：

* 
  **Windows 通知服务** - 请参阅[注册应用和接收云服务的凭据](/previous-versions/windows/apps/hh913756(v=win.10)#registering-your-app-and-receiving-the-credentials-for-your-cloud-service)和[应用程序注册门户](https://apps.dev.microsoft.com)。
* **Apple 推送通知服务** - 请参阅 [APNs 概述](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/APNSOverview.html)。
* **Google Cloud Messaging** - 请参阅 [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/)。

> [!NOTE]
> 如果使用 Firebase 使用 Android 凭据将通知推送到 iOS 设备，则需要提供 APN 凭据作为跨设备应用配置的一部分。 

## <a name="configure-a-cross-device-app-using-an-externally-hosted-json-file"></a>使用外部托管的 JSON 文件配置跨设备应用
跨设备应用 ID 表示为你拥有的域。 域指向作为域上托管的 JSON 文件存储或可通过 Windows 开发人员中心配置的特定于平台的应用 ID 的映射。 确定将用来表示跨设备应用 ID 的域后，将需要收集信息来配置关联的配置文件。 

### <a name="step-1-select-a-secure-domain-for-your-cross-device-app-id"></a>步骤 1：为跨设备应用 ID 选择安全域
跨设备应用 ID 表示为你拥有的域。 该域必须为顶级域或子域，且必须通过 TLS 保护。 例如：https://contoso.com 或 https://myapp.contoso.com，但不是 https://myapp.contoso.com/somepath。 每个跨设备应用必须具有唯一域（或子域）。 但是，根据要支持的跨平台行为决定将哪些应用与单个跨设备应用关联。 

例如，具有一套游戏应用的应用开发人员可能会对每个游戏应用使用单独的子域，以确保每个应用仅在跨设备和平台读取数据时可以继续执行的用户活动中订阅。 具有一套旨在协同工作的效率类应用的应用开发人员可能会对所有这些效率类应用使用单个域，以便应用能够跨设备启动该套件的成员。  

#### <a name="assert-domain-ownership-with-an-externally-hosted-json-file"></a>使用外部托管的 JSON 文件声明域所有权 
如果使用外部托管的 JSON 文件管理跨设备应用，则通过将 Microsoft 帐户或 Azure AD 应用 ID 包含在 cross-platform-app-identifiers 文件中来声明域所有权。 如果使用活动源 API 创建用户活动，则在发布过程中将验证你的域所有权。

系统将缓存 JSON 文件的内容以避免在域上生成频繁请求。 如果已配置，该服务将在评估何时刷新缓存时考虑 HTTP 缓存标头。 如果未配置，该服务将每 24 小时刷新一次。 

### <a name="step-2-collect-your-platform-specific-application-ids-and-construct-your-json-file"></a>步骤 2：收集特定于平台的应用程序 ID 并构造 JSON 文件
为将使用活动源和/或设备中继 API 的每个应用程序和平台收集特定于平台的应用程序 ID。 

将需要收集每个特定于平台的应用程序 ID，才能将其与跨设备应用标识关联。 使用外部托管的 JSON 文件，将需要收集每个特定于平台的应用的应用 ID，以配置为跨设备应用的一部分并将其组合为指定格式。 每个平台最多可以关联 10 个 ID。 

#### <a name="constructing-your-cross-platform-app-identifiers-file"></a>构造 cross-platform-app-identifiers 文件
JSON 文件本身必须命名为 **cross-platform-app-identifiers** 并托管在 HTTPS 域的根目录中。 该文件的内容是应用程序的支持平台与这些平台上的应用程序 ID 之间的映射的 JSON 数组。 构造该文件时，包括将使用 Project Rome API 的每个应用程序和平台的 JSON 对象。 
 
该文件将允许多个 JSON 对象具有相同平台标识符。 例如，iPhone 应用和 iPad 应用应作为单独的 JSON 对象列出，每个应用的平台值均为 iOS。 以下示例中显示了 Web 平台标识符。
 
不需要包括所有平台的 JSON 对象。 仅包括应用程序使用 Project Rome API 的平台的 JSON 对象。 例如，如果没有适用于 Android 平台的应用客户端，则不需要在 Android 文件中进行输入。
 
以下示例包含当前接受的所有有效平台标识符。 将删除包含无效平台值的 JSON 对象。  

```[
{"platform":"windows_universal", "application":"Microsoft.Contoso_8wekyb3d8bbwe"},
{"platform":"windows_win32", "application":"DefaultBrowser_NOPUBLISHERID!Microsoft.Contoso.Default"},
{"platform":"android","application":"com.example.myapp"},
{"platform":"ios", "application":"com.example.myapp"},
{"platform":"web", "application":"https://contoso.com"},
{"platform":"web", "application":"https://chat.contoso.com"},
{"platform":"msa", "application":"00000000603E0BF"},
{"platform":"msa", "application":"48932b46-98b1-4020-9be4-cc7a65643c9e"},
]
```

若要查找 ID，请执行以下操作：

* **windows_universal** - 为每个 UWP 应用提供 AUMID。 有关详细信息，请参阅[查找已安装应用 (Industry 8.1) 的应用程序用户模型 ID](/previous-versions/windows/embedded/dn449300(v=winembedded.82)) 和[应用程序](/uwp/schemas/appxpackage/appxmanifestschema/element-application)。
* **windows_win32** - 为每个应用提供 AUMID。 对于 win32 应用，将需要使用脚本来检索此信息。 有关详细信息，请参阅[查找已安装应用 (Industry 8.1) 的应用程序用户模型 ID](/previous-versions/windows/embedded/dn449300(v=winembedded.82))。
* **android** - 有关详细信息，请参阅 [更改包名称](https://developer.android.com/studio/build/application-id.html#change_the_package_name)。 
* **ios** - 有关详细信息，请参阅 [捆绑](https://developer.apple.com/documentation/foundation/bundle)和 [必需、可本地化和可编辑属性](https://help.apple.com/itunes-connect/developer/#/devfc3066644)。
* **msa** – 登录到 [应用程序注册门户](https://apps.dev.microsoft.com)。 可以查看任何应用的应用 ID/客户端 ID。 同时支持 Live SDK（十六进制值）和聚合应用 ID (GUID)。   

### <a name="step-3-configure-support-for-microsoft-account-or-azure-ad"></a>步骤 3：配置对 Microsoft 帐户或 Azure AD 的支持
若要启用跨设备体验，应用用户必须使用 Microsoft 帐户或 Azure AD 帐户进行登录。 你将提供应用 ID/客户端 ID 以在跨设备应用配置过程中支持身份验证，从而启用跨平台支持。 最多可提供 10 个实例。

```[
{"platform":"windows_universal", "application":"Microsoft.Contoso_8wekyb3d8bbwe"},
{"platform":"windows_win32", "application":"DefaultBrowser_NOPUBLISHERID!Microsoft.Contoso.Default"},
{"platform":"android","application":"com.example.myapp"},
{"platform":"ios", "application":"com.example.myapp"},
{"platform":"web", "application":"https://contoso.com"},
{"platform":"web", "application":"https://chat.contoso.com"},
{"platform":"msa", "application":"00000000603E0BF"},
{"platform":"msa", "application":"48932b46-98b1-4020-9be4-cc7a65643c9e"},
]
```

可以通过使用开发人员帐户登录到应用程序 [注册门户](https://apps.dev.microsoft.com) 来查找现有应用 ID/客户端 ID 或预配新 ID。 登录后，可以查看任何应用的应用 ID/客户端 ID。 同时支持 Live SDK（十六进制值）和聚合应用 ID (GUID)。 添加用于启用对 Microsoft 帐户或 Azure AD 的支持的 ID 时使用平台类型“msa”，如前一个示例中所示。  

> [!NOTE]
> 如果要生成支持 Azure AD 用户的应用程序，并且不使用通过应用程序 [注册门户](https://apps.dev.microsoft.com)颁发的聚合应用程序 ID，则需要为 Azure 应用的应用程序 ID 提供 GUID。 此类型的 ID 还应配置为平台类型“msa”。 

若要在 Azure 门户中查找租户的 GUID，请执行以下操作： 

1. 登录到 [Azure 门户](https://portal.azure.com)。
2. 选择“Azure Active Directory”。 
3. 在“管理”下，选择“应用注册”。
4. 从列表中选择你的应用。 可以在“概要”下查看应用程序 ID (GUID)。

#### <a name="encoding-the-cross-platform-app-identifiers-file"></a>对 cross-platform-app-identifiers 文件进行编码 
如果未看到活动在正确的本机应用程序中跨平台恢复，或无法读取由组中的所有成员发布的活动，则可能无法正确分析 JSON 文件。 输出此文件时，请确保使用“Unicode (UTF-8 无签名) - 代码页 65001”编码保存 cross-platform-app-identifiers 文件。

#### <a name="updating-the-cross-platform-app-identifiers-json-file"></a>更新 cross-platform-app-identifiers JSON 文件 
系统将缓存 JSON 文件的内容以避免在域上生成频繁请求。 如果已配置，该服务将在评估何时刷新缓存时考虑 HTTP 缓存标头。 如果未配置，该服务将每 24 小时刷新一次。 

## <a name="configure-your-app-client"></a>配置应用客户端 
如果使用适用于 Windows、iOS 或 Android 的客户端 API，将需要确保使用表示跨设备应用标识的主机值（例如，contoso.com）配置应用客户端。

### <a name="microsoft-graph-apps"></a>Microsoft Graph 应用 
如果你的应用使用 Microsoft Graph 中的活动源 API，则必须在 **activitySourceHost** 属性中提供主机值。 有关详细信息，请参阅[活动资源类型](/graph/api/resources/projectrome-activity)。

### <a name="universal-windows-apps"></a>通用 Windows 应用
如果具有 Windows 应用，将需要在发布数据之前在应用清单中配置主机值。 有关详细信息，请参阅 [uap5:UserActivity](/uwp/schemas/appxpackage/uapmanifestschema/element-uap5-useractivity)。 

<!-- Removing until we add the details.
### iOS & Android apps
*Details coming soon.*
-->

## <a name="maintain-your-cross-device-app-configuration"></a>维护跨设备应用配置
发布将生成用户活动的新应用程序时，请务必提前使用新配置值更新跨设备应用，以便发布的任何新活动与跨设备应用正确关联。 不会自动更新与在配置发生更改之前已发布的用户活动关联的跨设备应用配置。 使用旧配置对任何活动执行的更新操作将更新为文件上的最新版本。  

## <a name="troubleshooting"></a>疑难解答

下面是活动源 API 可能会出现的一些常见问题。

### <a name="activities-are-not-available-to-read-and-write-for-all-apps-in-the-cross-device-app-configuration"></a>无法读取和写入跨设备应用配置中的所有应用的活动
活动源 API 异步引入跨设备应用配置，因此在发布用户活动时配置错误可能不会很明显。 如果该服务由于 TLS 或格式错误而无法引入 JSON 文件，则已发布的任何活动将仅归于发布活动的应用 ID。 如果通过 Microsoft Graph 发布活动，则将使用 Microsoft 帐户应用 ID 授权对 Microsoft Graph 的请求。 如果通过客户端 API 发布活动，activity.applicationId 将仅记录发布活动的特定于平台的应用的 ID。 这将防止对跨设备应用配置中标识的任何其他特定于平台的应用中的活动执行读取和写入操作。 

### <a name="platform-will-not-initialize-on-android-or-ios"></a>平台不会在 Android 或 iOS 上进行初始化
适用于 Android 或 iOS 的设备中继 API 需要跨设备应用配置，才能实例化与 Android 或 iOS 应用的连接。 如果平台无法成功初始化，请确保已正确标识Microsoft 帐户应用 ID 和推送通知凭据，它们用于在 Windows 开发人员中心中配置跨设备并使用标识跨设备应用的域配置客户端应用的主机值。
