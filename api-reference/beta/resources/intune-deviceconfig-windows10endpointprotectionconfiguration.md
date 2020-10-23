---
title: windows10EndpointProtectionConfiguration 资源类型
description: 本主题提供由 Windows10EndpointProtectionConfiguration 资源公开的已声明方法、属性和关系的说明。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6ea18c512fa6b7cd96e333876184f4e7536a0d66
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724528"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>windows10EndpointProtectionConfiguration 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供由 Windows10EndpointProtectionConfiguration 资源公开的已声明方法、属性和关系的说明。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[List windows10EndpointProtectionConfigurations](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-list.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 集合|列出 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性和关系。|
|[Get windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-get.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|读取 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性和关系。|
|[Create windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-create.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|创建新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。|
|[Delete windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-delete.md)|无|删除 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)。|
|[Update windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-update.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|更新 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|布尔|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|适用于此策略的操作系统版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|dmaGuardDeviceEnumerationPolicy|[dmaGuardDeviceEnumerationPolicyType](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|此策略旨在提供针对支持外部 DMA 的设备的额外安全性。 通过它，可以更好地控制支持外部 DMA 的设备与 DMA 重新映射/设备内存隔离和沙盒不兼容的枚举。 仅当系统固件支持和启用内核 DMA 保护时，此策略才会生效。 内核 DMA 保护是一项平台功能，不能通过策略或最终用户进行控制。 在制造时，系统必须支持它。 若要检查系统是否支持内核 DMA 保护，请在 MSINFO32.exe 的摘要页中检查 "内核 DMA 保护" 字段。 可取值为：`deviceDefault`、`blockAll`、`allowAll`。|
|firewallRules|[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) 集合|配置防火墙规则设置。 此集合最多可包含150个元素。|
|userRightsAccessCredentialManagerAsTrustedCaller|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限由凭据管理器在备份/还原过程中使用。 如果为其他实体提供此权限，则用户保存的凭据可能会受到威胁。 仅支持 NotConfigured 和允许的状态|
|userRightsAllowAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定允许哪些用户和组通过网络连接到计算机。 支持的状态为 "允许"。|
|userRightsBlockAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限决定了阻止哪些用户和组通过网络连接到计算机。 支持状态块。|
|userRightsActAsPartOfTheOperatingSystem|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限允许进程在不进行身份验证的情况下模拟任何用户。 因此，该过程可以获得与该用户相同的本地资源的访问权限。 仅支持 NotConfigured 和允许的状态|
|userRightsLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以登录到计算机。 支持的状态 NotConfigured （允许） |
|userRightsDenyLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户无法登录到计算机。 状态 NotConfigured，受阻止 |
|userRightsBackupData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定在备份文件和目录时，哪些用户可以绕过文件、目录、注册表和其他持久对象权限。 仅支持 NotConfigured 和允许的状态|
|userRightsChangeSystemTime|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户和组可以更改计算机内部时钟上的时间和日期。 仅支持 NotConfigured 和允许的状态|
|userRightsCreateGlobalObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此安全设置确定用户是否可以创建可用于所有会话的全局对象。 可以创建全局对象的用户可能会影响在其他用户的会话下运行的进程，这可能导致应用程序故障或数据损坏。 仅支持 NotConfigured 和允许的状态|
|userRightsCreatePageFile|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户和组可以调用内部 API 来创建和更改页面文件的大小。 仅支持 NotConfigured 和允许的状态|
|userRightsCreatePermanentSharedObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限决定了进程可以使用哪些帐户使用对象管理器创建目录对象。 仅支持 NotConfigured 和允许的状态|
|userRightsCreateSymbolicLinks|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定用户是否可以从其登录到的计算机创建符号链接。 仅支持 NotConfigured 和允许的状态|
|userRightsCreateToken|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定进程在使用内部 API 创建访问令牌时，可以使用哪些用户/组来创建令牌，然后可以使用这些用户/组来获取对任何本地资源的访问权限。 仅支持 NotConfigured 和允许的状态|
|userRightsDebugPrograms|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以将调试程序附加到任何进程或内核。 仅支持 NotConfigured 和允许的状态|
|userRightsRemoteDesktopServicesLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定禁止哪些用户和组作为远程桌面服务客户端进行登录。 仅支持状态 NotConfigured 和阻止|
|userRightsDelegation|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以在用户或计算机对象上设置受信任委派设置。 仅支持 NotConfigured 和允许的状态。|
|userRightsGenerateSecurityAudits|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定进程可使用哪些帐户向安全日志中添加条目。 安全日志用于跟踪未经授权的系统访问。  仅支持 NotConfigured 和允许的状态。|
|userRightsImpersonateClient|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|将此用户权限分配给用户将允许代表该用户运行的程序模拟客户端。 如果此类型的模拟要求此用户权限，则可以防止未经授权的用户说服客户端连接到已创建的服务，然后模拟该客户端，这样可以将未经授权的用户的权限提升到管理级别或系统级别。 仅支持 NotConfigured 和允许的状态。|
|userRightsIncreaseSchedulingPriority|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些帐户可以使用具有对另一进程的 Write 属性访问权限的进程，以增加分配给其他进程的执行优先级。 仅支持 NotConfigured 和允许的状态。|
|userRightsLoadUnloadDrivers|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以在内核模式下将设备驱动程序或其他代码动态加载和卸载。 仅支持 NotConfigured 和允许的状态。|
|userRightsLockMemory|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些帐户可以使用进程将数据保存在物理内存中，这会阻止系统将数据分页到磁盘上的虚拟内存中。 仅支持 NotConfigured 和允许的状态。|
|userRightsManageAuditingAndSecurityLogs|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以为各个资源（如文件、Active Directory 对象和注册表项）指定对象访问审核选项。 仅支持 NotConfigured 和允许的状态。|
|userRightsManageVolumes|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户和组可以在某个卷（如远程碎片整理）上运行维护任务。 仅支持 NotConfigured 和允许的状态。|
|userRightsModifyFirmwareEnvironment|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限决定了可以修改固件环境值的用户。 仅支持 NotConfigured 和允许的状态。|
|userRightsModifyObjectLabels|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户帐户可以修改对象的完整性标签，例如，文件、注册表项或其他用户所拥有的进程。 仅支持 NotConfigured 和允许的状态。|
|userRightsProfileSingleProcess|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。 仅支持 NotConfigured 和允许的状态。|
|userRightsRemoteShutdown|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定允许哪些用户从网络上的远程位置关闭计算机。 误用此用户权限可能会导致拒绝服务。 仅支持 NotConfigured 和允许的状态。|
|userRightsRestoreData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定在还原备份的文件和目录时，哪些用户可以绕过文件、目录、注册表和其他持久对象权限，并确定哪些用户可以将任何有效的安全主体设置为对象的所有者。 仅支持 NotConfigured 和允许的状态。|
|userRightsTakeOwnership|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以获得系统中任何安全对象的所有权，包括 Active Directory 对象、文件和文件夹、打印机、注册表项、进程和线程。 仅支持 NotConfigured 和允许的状态。|
|xboxServicesEnableXboxGameSaveTask|布尔|此设置确定是否 (1) 或禁用 (0) 启用 xbox 游戏保存。|
|xboxServicesAccessoryManagementServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|此设置确定附件管理服务的启动类型是否为自动 (2) 、手动 (3) 禁用 (4) 。 默认：手动。 可取值为：`manual`、`automatic`、`disabled`。|
|xboxServicesLiveAuthManagerServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|此设置确定 Live Auth Manager 服务的启动类型是否为自动 (2) 、手动 (3) 禁用 (4) 。 默认：手动。 可取值为：`manual`、`automatic`、`disabled`。|
|xboxServicesLiveGameSaveServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|此设置确定 Live 游戏保存服务的启动类型是否为自动 (2) 、手动 (3) 禁用 (4) 。 默认：手动。 可取值为：`manual`、`automatic`、`disabled`。|
|xboxServicesLiveNetworkingServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|此设置确定网络服务的启动类型是否为自动 (2) 、手动 (3) 禁用 (4) 。 默认：手动。 可取值为：`manual`、`automatic`、`disabled`。|
|localSecurityOptionsBlockMicrosoftAccounts|布尔|阻止用户向此计算机添加新的 Microsoft 帐户。|
|localSecurityOptionsBlockRemoteLogonWithBlankPassword|布尔|启用不受密码保护的本地帐户从物理设备以外的位置进行登录。默认值为已启用|
|localSecurityOptionsDisableAdministratorAccount|布尔|确定是否启用或禁用本地管理员帐户。|
|localSecurityOptionsAdministratorAccountName|String|定义要与帐户 "管理员" 的 (SID) 的安全标识符相关联的不同帐户名称。|
|localSecurityOptionsDisableGuestAccount|布尔|确定来宾帐户是否已启用或已禁用。|
|localSecurityOptionsGuestAccountName|String|定义与帐户 "来宾" 的 "来宾" (SID) 的安全标识符相关联的其他帐户名称。|
|localSecurityOptionsAllowUndockWithoutHavingToLogon|布尔|阻止便携式计算机在无需登录的情况下被移除。|
|localSecurityOptionsBlockUsersInstallingPrinterDrivers|布尔|仅在将打印机驱动程序连接到共享打印机时，才将其限制为仅供管理员安装。|
|localSecurityOptionsBlockRemoteOpticalDriveAccess|布尔|如果启用此设置，则仅允许交互式登录用户访问 CD-ROM 媒体。|
|localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser|[localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|定义允许格式化和弹出可移动 NTFS 媒体的权限。 可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。|
|localSecurityOptionsMachineInactivityLimit|Int32|在屏幕保护程序运行之前，定义交互式桌面登录屏幕上不活动的最长分钟数。 有效值为0至9999|
|localSecurityOptionsMachineInactivityLimitInMinutes|Int32|在屏幕保护程序运行之前，定义交互式桌面登录屏幕上不活动的最长分钟数。 有效值为0至9999|
|localSecurityOptionsDoNotRequireCtrlAltDel|布尔|要求用户在登录前按 CTRL + ALT + DEL。|
|localSecurityOptionsHideLastSignedInUser|布尔|不显示上次在此设备上登录的用户的用户名。|
|localSecurityOptionsHideUsernameAtSignIn|布尔|在输入凭据后以及显示设备桌面之前，请勿显示登录此设备的人员的用户名。|
|localSecurityOptionsLogOnMessageTitle|String|为尝试登录的用户设置消息标题。|
|localSecurityOptionsLogOnMessageText|String|为尝试登录的用户设置消息文本。|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|布尔|阻止 PKU2U 对此设备的身份验证请求，以使用联机标识。|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool|布尔|LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体的 UI 帮助程序布尔值|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|String|编辑默认的安全描述符定义语言字符串，以允许或拒绝用户和组对 SAM 进行远程调用。|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|此安全设置允许客户端要求协商128位加密和/或 NTLMv2 会话安全性。 可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|此安全设置允许服务器要求协商128位加密和/或 NTLMv2 会话安全性。 可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。|
|lanManagerAuthenticationLevel|[lanManagerAuthenticationLevel](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|此安全设置确定用于网络登录的质询/响应身份验证协议。 可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。|
|lanManagerWorkstationDisableInsecureGuestLogons|布尔|如果启用，SMB 客户端将允许不安全的来宾登录。 如果未配置，SMB 客户端将拒绝不安全的来宾登录。|
|localSecurityOptionsClearVirtualMemoryPageFile|布尔|此安全设置确定在关闭系统时是否清除虚拟内存页面文件。|
|localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn|布尔|此安全设置确定是否可以在不登录 Windows 的情况下关闭计算机。|
|localSecurityOptionsAllowUIAccessApplicationElevation|布尔|允许 UIAccess 应用在不使用安全桌面的情况下提示提升。|
|localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations|布尔|将文件和注册表写入失败虚拟化到每个用户位置|
|localSecurityOptionsOnlyElevateSignedExecutables|布尔|对给定的可执行文件强制执行 PKI 证书路径验证，然后再允许运行该文件。|
|localSecurityOptionsAdministratorElevationPromptBehavior|[localSecurityOptionsAdministratorElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|在管理员审批模式中定义管理员的提升提示行为。 可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent` 或 `promptForConsentForNonWindowsBinaries`。|
|localSecurityOptionsStandardUserElevationPromptBehavior|[localSecurityOptionsStandardUserElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|定义标准用户的提升提示行为。 可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。|
|localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation|布尔|启用所有提升请求以转到交互式用户的桌面，而不是安全桌面。 使用管理员和标准用户的提示行为策略设置。|
|localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation|布尔|需要提升权限的应用程序安装将提示管理凭据。默认值为已启用|
|localSecurityOptionsAllowUIAccessApplicationsForSecureLocations|布尔|允许 UIAccess 应用在不使用安全桌面的情况下提示提升。默认值为已启用|
|localSecurityOptionsUseAdminApprovalMode|布尔|定义内置管理员帐户是使用管理员审批模式，还是运行所有具有完全管理员权限的应用程序。默认值为已启用|
|localSecurityOptionsUseAdminApprovalModeForAdministrators|布尔|定义是否启用管理员批准模式和所有 UAC 策略设置，默认为启用|
|localSecurityOptionsInformationShownOnLockScreen|[localSecurityOptionsInformationShownOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|配置在会话锁定时显示的用户信息。 如果未配置，则显示用户显示名称、域和用户名。 可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。|
|localSecurityOptionsInformationDisplayedOnLockScreen|[localSecurityOptionsInformationDisplayedOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|配置在会话锁定时显示的用户信息。 如果未配置，则显示用户显示名称、域和用户名。 可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。|
|localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees|布尔|此安全设置确定 SMB 客户端是否尝试协商 SMB 数据包签名。|
|localSecurityOptionsClientDigitallySignCommunicationsAlways|布尔|此安全设置确定 SMB 客户端组件是否需要数据包签名。|
|localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers|布尔|如果启用此安全设置，则允许服务器消息块 (SMB) 重定向器将纯文本密码发送到在身份验证过程中不支持密码加密的非 Microsoft SMB 服务器。|
|localSecurityOptionsDisableServerDigitallySignCommunicationsAlways|布尔|此安全设置确定 SMB 服务器组件是否需要数据包签名。|
|localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees|布尔|此安全设置确定 SMB 服务器是否将 SMB 数据包签名与请求的客户端协商。|
|localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares|布尔|默认情况下，此安全设置限制可匿名访问且可匿名访问的共享的命名管道设置对共享和管道的匿名访问权限|
|localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts|布尔|此安全设置确定将向计算机的匿名连接授予的其他权限。|
|localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares|布尔|此安全设置确定是否允许匿名用户执行某些活动，如枚举域帐户和网络共享的名称。|
|localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange|布尔|此安全设置确定是否在下一次更改密码时存储新密码 (LM) 哈希值。 默认情况下不存储它。|
|localSecurityOptionsSmartCardRemovalBehavior|[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|此安全设置确定将已登录用户的智能卡从智能卡读卡器中删除时发生的情况。 可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。|
|defenderSecurityCenterDisableAppBrowserUI|布尔|用于禁用应用程序和浏览器保护区域的显示。|
|defenderSecurityCenterDisableFamilyUI|布尔|用于禁用 "家庭选项" 区域的显示。|
|defenderSecurityCenterDisableHealthUI|布尔|用于禁用设备性能和运行状况区域的显示。|
|defenderSecurityCenterDisableNetworkUI|布尔|用于禁用防火墙和网络防护区域的显示。|
|defenderSecurityCenterDisableVirusUI|布尔|用于禁用病毒和威胁防护区域的显示。|
|defenderSecurityCenterDisableAccountUI|布尔|用于禁用帐户保护区域的显示。|
|defenderSecurityCenterDisableClearTpmUI|布尔|用于禁用 "清除 TPM" 按钮的显示。|
|defenderSecurityCenterDisableHardwareUI|布尔|用于禁用硬件保护区域的显示。|
|defenderSecurityCenterDisableNotificationAreaUI|布尔|用于禁用通知区域控件的显示。 用户需要注销并登录或重新启动计算机，此设置才会生效。|
|defenderSecurityCenterDisableRansomwareUI|布尔|用于禁用勒索软件防护区域的显示。 |
|defenderSecurityCenterDisableSecureBootUI|布尔|用于在 "设备安全性" 下禁用安全引导区域的显示。|
|defenderSecurityCenterDisableTroubleshootingUI|布尔|用于在 "设备安全性" 下禁用安全过程故障排除的显示。|
|defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI|布尔|用于在检测到易受攻击的固件时禁用显示更新 TPM 固件。|
|defenderSecurityCenterOrganizationDisplayName|String|向用户显示的公司名称。|
|defenderSecurityCenterHelpEmail|String|向用户显示的电子邮件地址。|
|defenderSecurityCenterHelpPhone|String|向用户显示的电话号码或 Skype ID。|
|defenderSecurityCenterHelpURL|String|"帮助" 门户 URL 将向用户显示。|
|defenderSecurityCenterNotificationsFromApp|[defenderSecurityCenterNotificationsFromAppType](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|要从应用程序的显示区域中显示的通知。 可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。|
|defenderSecurityCenterITContactDisplay|[defenderSecurityCenterITContactDisplayType](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|配置向最终用户显示 IT 联系人信息的位置。 可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。|
|windowsDefenderTamperProtection|[windowsDefenderTamperProtectionOptions](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|配置 windows defender TamperProtection 设置。 可取值为：`notConfigured`、`enable`、`disable`。|
|firewallBlockStatefulFTP|Boolean|阻止到设备的有状态 FTP 连接|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。 这是一个时间段，在此之后安全关联将过期并被删除。 有效值为 300 至 3600|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|选择要使用的预共享密钥编码。 可取值为：`deviceDefault`、`none`、`utF8`。|
|firewallIPSecExemptionsNone|布尔|将 IPSec 免除配置为 "无例外"|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码|
|firewallIPSecExemptionsAllowICMP|Boolean|配置 IPSec 免除项以允许 ICMP|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码|
|firewallIPSecExemptionsAllowDHCP|Boolean|配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|指定如何强制执行证书吊销列表。 可取值为：`deviceDefault`、`none`、`attempt`、`require`。|
|firewallMergeKeyingModuleSettings|Boolean|如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|配置如何在隧道网关应用场景中应用数据包排队。 可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|配置域网络的防火墙配置文件设置|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|配置公用网络的防火墙配置文件设置|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|配置专用网络的防火墙配置文件设置|
|defenderAdobeReaderLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|值，该值指示 Adobe Reader 创建子进程的行为。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderAttackSurfaceReductionExcludedPaths|String 集合|要从攻击面减少规则中排除的 exe 文件和文件夹的列表|
|defenderOfficeAppsOtherProcessInjectionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|值，该值指示插入到其他进程中的 Office 应用程序的行为。 可取值为：`userDefined`、`block`、`auditMode`。|
|defenderOfficeAppsOtherProcessInjection|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|值，该值指示插入到其他进程中的 Office 应用程序的行为。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderOfficeCommunicationAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|值，该值指示 Office 通信应用程序（包括 Microsoft Outlook）在创建子进程时的行为。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderOfficeAppsExecutableContentCreationOrLaunchType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|值，该值指示 Office 应用程序/宏创建或启动可执行内容的行为。 可取值为：`userDefined`、`block`、`auditMode`。|
|defenderOfficeAppsExecutableContentCreationOrLaunch|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|值，该值指示 Office 应用程序/宏创建或启动可执行内容的行为。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderOfficeAppsLaunchChildProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|值，该值指示 Office 应用程序启动子进程的行为。 可取值为：`userDefined`、`block`、`auditMode`。|
|defenderOfficeAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|值，该值指示 Office 应用程序启动子进程的行为。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderOfficeMacroCodeAllowWin32ImportsType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|值，该值指示从 Office 中的宏代码的 Win32 导入行为。 可取值为：`userDefined`、`block`、`auditMode`。|
|defenderOfficeMacroCodeAllowWin32Imports|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|值，该值指示从 Office 中的宏代码的 Win32 导入行为。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderScriptObfuscatedMacroCodeType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|值，该值指示模糊的 js/vbs/ps/宏代码的行为。 可取值为：`userDefined`、`block`、`auditMode`。|
|defenderScriptObfuscatedMacroCode|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|值，该值指示模糊的 js/vbs/ps/宏代码的行为。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderScriptDownloadedPayloadExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|值，该值指示从 Internet 下载的 js/vbs 执行负载的行为。 可取值为：`userDefined`、`block`、`auditMode`。|
|defenderScriptDownloadedPayloadExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|值，该值指示从 Internet 下载的 js/vbs 执行负载的行为。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderPreventCredentialStealingType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|值，该值指示是否允许从 Windows 本地安全机构子系统中盗取凭据。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderProcessCreationType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|一个值，该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。 可取值为：`userDefined`、`block`、`auditMode`。|
|defenderProcessCreation|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|一个值，该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderUntrustedUSBProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示对从 USB 运行的不受信任和未签名进程的响应的值。 可取值为：`userDefined`、`block`、`auditMode`。|
|defenderUntrustedUSBProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示对从 USB 运行的不受信任和未签名进程的响应的值。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderUntrustedExecutableType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。 可取值为：`userDefined`、`block`、`auditMode`。|
|defenderUntrustedExecutable|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderEmailContentExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|值，该值指示是否应从电子邮件 (web 邮件) 中删除可执行内容 (exe、dll、ps、js、vbs 等) 的执行情况。 可取值为：`userDefined`、`block`、`auditMode`。|
|defenderEmailContentExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|值，该值指示是否应从电子邮件 (web 邮件) 中删除可执行内容 (exe、dll、ps、js、vbs 等) 的执行情况。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderAdvancedRansomewareProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示使用针对 ransomeware 的高级防护的值。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderGuardMyFoldersType|[folderProtectionType](../resources/intune-deviceconfig-folderprotectiontype.md)|值，该值指示受保护文件夹的行为。 可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification`。|
|defenderGuardedFoldersAllowedAppPaths|String 集合|允许访问受保护文件夹的 exe 路径列表|
|defenderAdditionalGuardedFolders|String 集合|要添加到受保护文件夹列表的文件夹路径列表|
|defenderNetworkProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|值，该值指示 NetworkProtection 的行为。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderExploitProtectionXml|Binary|包含有关 Exploit Protection 详细信息的 xml 内容。|
|defenderExploitProtectionXmlFileName|String|从中获取 DefenderExploitProtectionXml 的文件的名称。|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|指示是否阻止用户覆盖 Exploit Protection 设置。|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|使管理员能够选择在设备上允许哪些类型的应用。 可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。|
|deviceGuardLocalSystemAuthorityCredentialGuardSettings|[deviceGuardLocalSystemAuthorityCredentialGuardType](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|如果平台安全级别具有安全启动和基于虚拟化的安全性均已启用，则打开 Credential Guard。 可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`、`disable`。|
|deviceGuardEnableVirtualizationBasedSecurity|布尔|打开基于虚拟化的安全性 (VBS) 。|
|deviceGuardEnableSecureBootWithDMA|布尔|此属性将在5月2019中被弃用，并将替换为属性 DeviceGuardSecureBootWithDMA。 指定是否在下次重新启动时启用平台安全级别。|
|deviceGuardSecureBootWithDMA|[secureBootWithDMAType](../resources/intune-deviceconfig-securebootwithdmatype.md)|指定是否在下次重新启动时启用平台安全级别。 可取值为：`notConfigured`、`withoutDMA`、`withDMA`。|
|deviceGuardLaunchSystemGuard|[启用](../resources/intune-shared-enablement.md)|允许 IT 管理员配置启动 "系统防护"。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|smartScreenEnableInShell|Boolean|允许 IT 管理员配置适用于 Windows 的 SmartScreen。|
|smartScreenBlockOverrideForFiles|Boolean|允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。|
|applicationGuardEnabled|Boolean|启用 Windows Defender 应用程序防护|
|applicationGuardEnabledOptions|[applicationGuardEnabledOptions](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|为较新的 Windows 版本启用 Windows Defender 应用程序防护。 可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。|
|applicationGuardBlockFileTransfer|[applicationGuardBlockFileTransferType](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|阻止剪贴板传输图像文件、文本文件或二者都不。 可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。|
|applicationGuardBlockNonEnterpriseContent|Boolean|阻止企业站点加载非企业内容，例如第三方插件|
|applicationGuardAllowPersistence|Boolean|允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据|
|applicationGuardForceAuditing|Boolean|强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）|
|applicationGuardBlockClipboardSharing|[applicationGuardBlockClipboardSharingType](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。 可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。|
|applicationGuardAllowPrintToPDF|Boolean|允许从容器打印为 PDF 格式|
|applicationGuardAllowPrintToXPS|Boolean|允许从容器打印为 XPS 格式|
|applicationGuardAllowPrintToLocalPrinters|Boolean|允许从容器打印到本地打印机|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|允许从容器打印到网络打印机|
|applicationGuardAllowVirtualGPU|布尔|允许应用程序防护使用虚拟 GPU|
|applicationGuardAllowFileSaveOnHost|布尔|允许用户从应用程序防护容器中的边缘下载文件并将其保存在主机文件系统上|
|bitLockerAllowStandardUserEncryption|布尔|允许管理员允许标准用户在 Azure AD 加入过程中启用 encrpytion。|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|允许管理员禁用对用户计算机上其他磁盘加密的警告提示。|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|允许管理员要求使用 BitLocker 开启加密功能。 此策略仅适用于移动 SKU。|
|bitLockerEncryptDevice|Boolean|允许管理员要求使用 BitLocker 开启加密功能。|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|BitLocker 系统驱动器策略。|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|BitLocker 固定驱动器策略。|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|BitLocker 可移动驱动器策略。|
|bitLockerRecoveryPasswordRotation|[bitLockerRecoveryPasswordRotationType](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|此设置在 OS 驱动器恢复后启动客户端驱动的恢复密码轮替， (使用 bootmgr 或 WinRE) 。 可取值为：`notConfigured`、`disabled`、`enabledForAzureAd`、`enabledForAzureAdAndHybrid`。|
|defenderDisableScanArchiveFiles|布尔|允许或禁止扫描存档。|
|defenderAllowScanArchiveFiles|布尔|允许或禁止扫描存档。|
|defenderDisableBehaviorMonitoring|布尔|允许或禁止 Windows Defender 行为监控功能。|
|defenderAllowBehaviorMonitoring|布尔|允许或禁止 Windows Defender 行为监控功能。|
|defenderDisableCloudProtection|布尔|为最大限度地保护你的电脑，Windows Defender 将向 Microsoft 发送有关发现的任何问题的信息。 Microsoft 将分析该信息，详细了解影响您和其他客户的问题，并提供改进的解决方案。|
|defenderAllowCloudProtection|布尔|为最大限度地保护你的电脑，Windows Defender 将向 Microsoft 发送有关发现的任何问题的信息。 Microsoft 将分析该信息，详细了解影响您和其他客户的问题，并提供改进的解决方案。|
|defenderEnableScanIncomingMail|布尔|允许或禁止扫描电子邮件。|
|defenderEnableScanMappedNetworkDrivesDuringFullScan|布尔|允许或禁止对映射的网络驱动器进行完全扫描。|
|defenderDisableScanRemovableDrivesDuringFullScan|布尔|允许或禁止对可移动驱动器进行完全扫描。 在快速扫描过程中，可能仍会扫描可移动驱动器。|
|defenderAllowScanRemovableDrivesDuringFullScan|布尔|允许或禁止对可移动驱动器进行完全扫描。 在快速扫描过程中，可能仍会扫描可移动驱动器。|
|defenderDisableScanDownloads|布尔|允许或禁止 Windows Defender IOAVP 保护功能。|
|defenderAllowScanDownloads|布尔|允许或禁止 Windows Defender IOAVP 保护功能。|
|defenderDisableIntrusionPreventionSystem|布尔|允许或禁止 Windows Defender 入侵防护功能。|
|defenderAllowIntrusionPreventionSystem|布尔|允许或禁止 Windows Defender 入侵防护功能。|
|defenderDisableOnAccessProtection|布尔|允许或禁止 Windows Defender 访问保护功能。|
|defenderAllowOnAccessProtection|布尔|允许或禁止 Windows Defender 访问保护功能。|
|defenderDisableRealTimeMonitoring|布尔|允许或禁止 Windows Defender 实时监视功能。|
|defenderAllowRealTimeMonitoring|布尔|允许或禁止 Windows Defender 实时监视功能。|
|defenderDisableScanNetworkFiles|布尔|允许或禁止扫描网络文件。|
|defenderAllowScanNetworkFiles|布尔|允许或禁止扫描网络文件。|
|defenderDisableScanScriptsLoadedInInternetExplorer|布尔|允许或禁止 Windows Defender 脚本扫描功能。|
|defenderAllowScanScriptsLoadedInInternetExplorer|布尔|允许或禁止 Windows Defender 脚本扫描功能。|
|defenderBlockEndUserAccess|Boolean|允许或禁止用户访问 Windows Defender UI。 如果不允许，将同时禁止显示所有 Windows Defender 通知。|
|defenderAllowEndUserAccess|布尔|允许或禁止用户访问 Windows Defender UI。 如果不允许，将同时禁止显示所有 Windows Defender 通知。|
|defenderScanMaxCpuPercentage|Int32|表示 Windows Defender 扫描 (的平均 CPU 负载因子，以百分比) 为单位）。 默认值为 50。 有效值为 0 至 100|
|defenderCheckForSignaturesBeforeRunningScan|布尔|通过此策略设置，您可以管理在运行扫描前是否检查新病毒和间谍软件定义。|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|在 Windows 10 版本1709中添加。 此策略设置确定 Windows Defender 防病毒在阻止和扫描可疑文件时的积极程度。 值类型为 integer。 此功能需要启用 "加入 Microsoft MAPS" 设置，才能正常运行。 可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。|
|defenderCloudExtendedTimeoutInSeconds|Int32|在 Windows 10 版本1709中添加。 此功能允许 Windows Defender 防病毒阻止可疑文件长达60秒，并在云中对其进行扫描以确保其安全。 值类型为 integer，范围为 0-50。 此功能依赖于其他三个映射设置必须全部启用-"配置 ' 在首次看到时阻止 '" 功能; "加入 Microsoft MAPS ";"需要进一步分析时发送文件示例"。 有效值为 0 至 50|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|将隔离项目存储在系统上的时间段 (天) 。 有效值为 0 至 90|
|defenderDisableCatchupFullScan|布尔|通过此策略设置，您可以配置计划完全扫描的追赶扫描。 追赶扫描是由于错过了定期计划的扫描而启动的扫描。 通常情况下，这些计划扫描会因计算机在计划时间关闭而丢失。|
|defenderDisableCatchupQuickScan|布尔|通过此策略设置，您可以配置计划快速扫描的追赶扫描。 追赶扫描是由于错过了定期计划的扫描而启动的扫描。 通常情况下，这些计划扫描会因计算机在计划时间关闭而丢失。|
|defenderEnableLowCpuPriority|布尔|通过此策略设置，您可以启用或禁用计划扫描的 CPU 低优先级。|
|defenderFileExtensionsToExclude|String 集合|要从扫描和实时保护中排除的文件扩展名。|
|defenderFilesAndFoldersToExclude|String 集合|要从扫描和实时保护中排除的文件和文件夹。|
|defenderProcessesToExclude|String 集合|要从扫描和实时保护中排除的进程。|
|defenderPotentiallyUnwantedAppAction|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|已添加到 Windows 10 版本 1607 中。 指定 (PUAs) 的可能有害的应用程序的检测级别。 Windows Defender 会在下载可能不需要的软件或尝试在你的计算机上安装自己时向你发出警告。 可取值为：`userDefined`、`enable`、`auditMode`。|
|defenderScanDirection|[defenderRealtimeScanDirection](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|控制应监视的文件集。 可取值为：`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|选择是否执行快速扫描或完全扫描。 可取值为：`userDefined`、`disabled`、`quick`、`full`。|
|defenderScheduledQuickScanTime|TimeOfDay|选择 Windows Defender 快速扫描应在一天的哪一时间运行。 例如，值为 0 = 12：00AM，值为 60 = 1：00AM，值 120 = 2：00，等等，最高为 1380 = 11：00PM 的值。 默认值为120|
|defenderScheduledScanDay|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|选择 Windows Defender 扫描应运行的日期。 可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan`。|
|defenderScheduledScanTime|TimeOfDay|选择 Windows Defender 扫描应在一天的哪一时间运行。|
|defenderSignatureUpdateIntervalInHours|Int32|指定将用于检查签名的 (时间间隔（以) 小时为单位），ScheduleDay 和 ScheduleTime，而不是使用和。将根据间隔设置检查是否有新的签名。 有效值为 0 至 24|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|检查 Windows Defender 中的用户同意级别以发送数据。 可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|允许管理员指定任何有效的威胁严重级别和相应的默认操作 ID 进行。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|按用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "dmaGuardDeviceEnumerationPolicy": "String",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "String",
      "description": "String",
      "packageFamilyName": "String",
      "filePath": "String",
      "serviceName": "String",
      "protocol": 1024,
      "localPortRanges": [
        "String"
      ],
      "remotePortRanges": [
        "String"
      ],
      "localAddressRanges": [
        "String"
      ],
      "remoteAddressRanges": [
        "String"
      ],
      "profileTypes": "String",
      "action": "String",
      "trafficDirection": "String",
      "interfaceTypes": "String",
      "edgeTraversal": "String",
      "localUserAuthorizations": "String"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDenyLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "String",
  "xboxServicesLiveAuthManagerServiceStartupMode": "String",
  "xboxServicesLiveGameSaveServiceStartupMode": "String",
  "xboxServicesLiveNetworkingServiceStartupMode": "String",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "String",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "String",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "String",
  "localSecurityOptionsMachineInactivityLimit": 1024,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 1024,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "String",
  "localSecurityOptionsLogOnMessageText": "String",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "String",
  "lanManagerAuthenticationLevel": "String",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "String",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "String",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "String",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "String",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "String",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "String",
  "defenderSecurityCenterHelpEmail": "String",
  "defenderSecurityCenterHelpPhone": "String",
  "defenderSecurityCenterHelpURL": "String",
  "defenderSecurityCenterNotificationsFromApp": "String",
  "defenderSecurityCenterITContactDisplay": "String",
  "windowsDefenderTamperProtection": "String",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsNone": true,
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "String",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "String",
  "defenderOfficeAppsOtherProcessInjection": "String",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "String",
  "defenderOfficeAppsLaunchChildProcessType": "String",
  "defenderOfficeAppsLaunchChildProcess": "String",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "String",
  "defenderOfficeMacroCodeAllowWin32Imports": "String",
  "defenderScriptObfuscatedMacroCodeType": "String",
  "defenderScriptObfuscatedMacroCode": "String",
  "defenderScriptDownloadedPayloadExecutionType": "String",
  "defenderScriptDownloadedPayloadExecution": "String",
  "defenderPreventCredentialStealingType": "String",
  "defenderProcessCreationType": "String",
  "defenderProcessCreation": "String",
  "defenderUntrustedUSBProcessType": "String",
  "defenderUntrustedUSBProcess": "String",
  "defenderUntrustedExecutableType": "String",
  "defenderUntrustedExecutable": "String",
  "defenderEmailContentExecutionType": "String",
  "defenderEmailContentExecution": "String",
  "defenderAdvancedRansomewareProtectionType": "String",
  "defenderGuardMyFoldersType": "String",
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderNetworkProtectionType": "String",
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "String",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "String",
  "deviceGuardLaunchSystemGuard": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "String",
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "String",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "String",
    "startupAuthenticationTpmPinUsage": "String",
    "startupAuthenticationTpmKeyUsage": "String",
    "startupAuthenticationTpmPinAndKeyUsage": "String",
    "minimumPinLength": 1024,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "String",
    "prebootRecoveryUrl": "String"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  },
  "bitLockerRecoveryPasswordRotation": "String",
  "defenderDisableScanArchiveFiles": true,
  "defenderAllowScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderAllowBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderAllowCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderAllowScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderAllowScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderAllowIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderAllowOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderAllowRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderAllowScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderAllowScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderAllowEndUserAccess": true,
  "defenderScanMaxCpuPercentage": 1024,
  "defenderCheckForSignaturesBeforeRunningScan": true,
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeoutInSeconds": 1024,
  "defenderDaysBeforeDeletingQuarantinedMalware": 1024,
  "defenderDisableCatchupFullScan": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderEnableLowCpuPriority": true,
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderScanDirection": "String",
  "defenderScanType": "String",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderScheduledScanDay": "String",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderSignatureUpdateIntervalInHours": 1024,
  "defenderSubmitSamplesConsentType": "String",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "String",
    "moderateSeverity": "String",
    "highSeverity": "String",
    "severeSeverity": "String"
  }
}
```





