---
title: windows10EndpointProtectionConfiguration 资源类型
description: 本主题提供由 Windows10EndpointProtectionConfiguration 资源公开的已声明方法、属性和关系的说明。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0095e0c05d0ede8fe2d631151040d33bc9158894
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788210"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>windows10EndpointProtectionConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供由 Windows10EndpointProtectionConfiguration 资源公开的已声明方法、属性和关系的说明。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
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
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|dmaGuardDeviceEnumerationPolicy|[dmaGuardDeviceEnumerationPolicyType](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|此策略旨在针对支持外部 DMA 的设备提供额外的安全性。 它允许对与 DMA 重新映射/设备内存隔离和沙盒不兼容的外部支持 DMA 的设备枚举进行更多控制。 此策略仅在系统固件支持并启用内核 DMA 保护时生效。 内核 DMA 保护是一项平台功能，无法通过策略或最终用户控制。 它在制造时必须受系统支持。 若要检查系统是否支持内核 DMA 保护，请检查内核 DMA 保护字段（在 MSINFO32.exe 的摘要页中）。 可取值为：`deviceDefault`、`blockAll`、`allowAll`。|
|firewallRules|[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) 集合|配置防火墙规则设置。 此集合最多可包含 150 个元素。|
|userRightsAccessCredentialManagerAsTrustedCaller|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限在备份/还原期间由凭据管理器使用。 如果向其他实体授予此权限，则用户保存的凭据可能会泄露。 仅支持状态 NotConfigured 和 Allowed|
|userRightsAllowAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定允许哪些用户和组通过网络连接到计算机。 支持允许的状态。|
|userRightsBlockAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定阻止哪些用户和组通过网络连接到计算机。 支持状态块。|
|userRightsActAsPartOfTheOperatingSystem|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限允许进程模拟任何用户而不进行身份验证。 因此，该过程可以获得与该用户相同的本地资源的访问权限。 仅支持状态 NotConfigured 和 Allowed|
|userRightsLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以登录到计算机。 支持状态 NotConfigured、Allowed |
|userRightsDenyLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户无法登录计算机。 状态 NotConfigured、Blocked 受支持 |
|userRightsBackupData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户在备份文件和目录时可以绕过文件、目录、注册表和其他永久对象权限。 仅支持状态 NotConfigured 和 Allowed|
|userRightsChangeSystemTime|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户和组可以更改计算机内部时钟的时间和日期。 仅支持状态 NotConfigured 和 Allowed|
|userRightsCreateGlobalObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此安全性设置确定用户能否创建可用于所有会话的全局对象。 可以创建全局对象的用户可能会影响在其他用户的会话下运行的进程，这可能会导致应用程序失败或数据损坏。 仅支持状态 NotConfigured 和 Allowed|
|userRightsCreatePageFile|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户和组可以调用内部 API 来创建和更改页面文件的大小。 仅支持状态 NotConfigured 和 Allowed|
|userRightsCreatePermanentSharedObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定进程可以使用哪些帐户来创建使用对象管理器的目录对象。 仅支持状态 NotConfigured 和 Allowed|
|userRightsCreateSymb创建Links|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定用户能否从登录的计算机创建符号链接。 仅支持状态 NotConfigured 和 Allowed|
|userRightsCreateToken|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定进程可以使用哪些用户/组来创建令牌，然后当进程使用内部 API 创建访问令牌时，该令牌可用于获取对任意本地资源的访问权限。 仅支持状态 NotConfigured 和 Allowed|
|userRightsDebugPrograms|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以将调试器附加到任何进程或内核。 仅支持状态 NotConfigured 和 Allowed|
|userRightsRemoteDesktopServicesLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定禁止哪些用户和组以远程桌面服务客户端登录。 仅支持状态 NotConfigured 和 Blocked|
|userRightsDelegation|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以在用户或计算机对象上设置"受信任的委派"设置。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsGenerateSecurityAudits|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定进程可以使用哪些帐户向安全日志添加条目。 安全日志用于跟踪未经授权的系统访问。  仅支持状态 NotConfigured 和 Allowed。|
|userRightsImpersonateClient|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|向用户分配此用户权限允许代表该用户运行的程序模拟客户端。 要求此用户具有此用户权限进行这种模拟可防止未经授权的用户冒充客户端连接到他们创建的服务，然后模拟该客户端，这会将未授权用户的权限提升到管理级别或系统级别。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsIncreaseSchedulingPriority|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些帐户可以使用具有对另一个进程的 Write Property 访问权限的进程来增加分配给另一个进程的执行优先级。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsLoadUnloadDrivers|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以在内核模式下动态加载和卸载设备驱动程序或其他代码。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsLockMemory|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些帐户可以使用进程将数据保留于物理内存中，这可以防止系统将数据分页到磁盘上的虚拟内存中。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsManageAuditingAndSecurityLogs|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以为单个资源（如文件、Active Directory 对象和注册表项）指定对象访问审核选项。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsManageVolumes|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户和组可以在卷上运行维护任务，例如远程碎片整理。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsModifyFirmwareEnvironment|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定可以修改固件环境值的用户。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsModifyObjectLabels|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户帐户可以修改对象（如文件、注册表项或其他用户拥有的进程）的完整性标签。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsProfileSingleProcess|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsRemoteShutdown|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定允许哪些用户从网络远程位置关闭计算机。 滥用此用户权限可能会导致拒绝服务。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsRestoreData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户在还原备份的文件和目录时可以绕过文件、目录、注册表和其他永久对象权限，并确定哪些用户可以将任何有效的安全主体设置为对象的所有者。 仅支持状态 NotConfigured 和 Allowed。|
|userRightsOwnership|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|此用户权限确定哪些用户可以获得系统中任何安全对象的所有权，包括 Active Directory 对象、文件和文件夹、打印机、注册表项、进程和线程。 仅支持状态 NotConfigured 和 Allowed。|
|xboxServicesEnableXboxGameSaveTask|Boolean|此设置确定 xbox 游戏保存是在 1 (1) 还是从 0 (禁用) 。|
|xboxServicesAccessoryManagementServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|此设置确定附件管理服务的启动类型是自动 (2) 、手动 (3) 、禁用 (4) 。 默认值：手动。 可取值为：`manual`、`automatic`、`disabled`。|
|xboxServicesLiveAuthManagerServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|此设置确定 Live Auth Manager 服务的启动类型是自动 (2) 、手动 (3) 、禁用 (4) 。 默认值：手动。 可取值为：`manual`、`automatic`、`disabled`。|
|xboxServicesLiveGameSaveServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|此设置确定 Live Game 保存服务的启动类型是否为 4 (2) 、手动 (3) 、禁用 (4) 。 默认值：手动。 可取值为：`manual`、`automatic`、`disabled`。|
|xboxServicesLiveNetworkingServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|此设置确定网络服务的启动类型是 4 (2) 、手动 (3) 、禁用 (4) 。 默认值：手动。 可取值为：`manual`、`automatic`、`disabled`。|
|localSecurityOptionsBlockMicrosoftAccounts|Boolean|阻止用户向此计算机添加新的 Microsoft 帐户。|
|localSecurityOptionsBlockRemoteLogonWithBlankPassword|Boolean|启用未受密码保护的本地帐户，以便从物理设备外的位置登录。默认为启用|
|localSecurityOptionsDisableAdministratorAccount|Boolean|确定是启用还是禁用本地管理员帐户。|
|localSecurityOptionsAdministratorAccountName|String|定义一个不同的帐户名称，以与"管理员" (SID) 安全标识符相关联。|
|localSecurityOptionsDisableGuestAccount|Boolean|确定是否启用或禁用来宾帐户。|
|localSecurityOptionsGuestAccountName|String|定义一个不同的帐户名称，以与"来宾" (SID) 关联的安全标识符。|
|localSecurityOptionsAllowUndockWithoutHavingToLogon|Boolean|防止便携计算机在无需登录的情况下被移除。|
|localSecurityOptionsBlockUsersInstallingPrinterDrivers|Boolean|限制为仅将打印机驱动程序安装为连接到共享打印机的一部分。|
|localSecurityOptionsBlockRemoteOpticalDriveAccess|Boolean|启用这些设置仅允许以交互方式登录的用户访问 CD-ROM 媒体。|
|localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser|[localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|定义允许谁格式化和弹出可移动 NTFS 媒体。 可能的值是：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。|
|localSecurityOptionsMachineInactivityLimit|Int32|定义交互式桌面登录屏幕上不活动的最大分钟数，直到屏幕保护程序运行。 有效值为 0 到 9999|
|localSecurityOptionsMachineInactivityLimitInMinutes|Int32|定义交互式桌面登录屏幕上不活动的最大分钟数，直到屏幕保护程序运行。 有效值为 0 到 9999|
|localSecurityOptionsDoNotRequireCtrlAltDel|Boolean|要求在用户登录前按 Ctrl+Alt+DEL。|
|localSecurityOptionsHideLastSignedInUser|布尔值|不显示最后一个登录此设备的用户的用户名。|
|localSecurityOptionsHideUsernameAtSignIn|布尔值|输入凭据后和显示设备桌面之前，不显示登录此设备的用户的用户名。|
|localSecurityOptionsLogOnMessageTitle|String|为尝试登录的用户设置消息标题。|
|localSecurityOptionsLogOnMessageText|String|设置尝试登录的用户的消息文本。|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|布尔值|阻止对此设备的 PKU2U 身份验证请求使用联机标识。|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool|Boolean|LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体的 UI 帮助程序布尔值|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|String|编辑默认安全描述符定义语言字符串以允许或拒绝用户和组对 SAM 进行远程调用。|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|此安全性设置允许客户端要求协商 128 位加密和/或 NTLMv2 会话安全性。 可能的值是：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|此安全性设置允许服务器要求协商 128 位加密和/或 NTLMv2 会话安全性。 可能的值是：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。|
|lanManagerAuthenticationLevel|[lanManagerAuthenticationLevel](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|此安全性设置确定用于网络登录的质询/响应身份验证协议。 可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。|
|lanManagerWorkstationDisableInsecureGuestLogons|Boolean|如果启用，SMB 客户端将允许不安全的来宾徽标。 如果未配置，SMB 客户端将拒绝不安全的来宾徽标。|
|localSecurityOptionsClearVirtualMemoryPageFile|Boolean|此安全设置确定是否在系统关闭时清除虚拟内存页面文件。|
|localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn|Boolean|此安全设置确定是否可以关闭计算机，而不必登录到Windows。|
|localSecurityOptionsAllowUIAccessApplicationElevation|Boolean|允许 UIAccess 应用在没有使用安全桌面的情况下提示提升。|
|localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations|Boolean|将文件和注册表写入故障虚拟化到每个用户位置|
|localSecurityOptionsOnlyElevateSignedExecutables|Boolean|在允许运行给定可执行文件之前，对该文件强制执行 PKI 证书路径验证。|
|localSecurityOptionsAdministratorElevationPromptBehavior|[localSecurityOptionsAdministratorElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|定义管理员审批模式下管理员的提升权限提示行为。 可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent` 或 `promptForConsentForNonWindowsBinaries`。|
|localSecurityOptionsStandardUserElevationPromptBehavior|[localSecurityOptionsStandardUserElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|定义标准用户的提升权限提示的行为。 可能的值是：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。|
|localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation|Boolean|启用所有提升请求以转到交互式用户的桌面，而不是安全桌面。 使用管理员和标准用户的提示行为策略设置。|
|localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation|Boolean|需要提升特权的应用安装将提示输入管理员凭据。默认为启用|
|localSecurityOptionsAllowUIAccessApplicationsForSecureLocations|Boolean|允许 UIAccess 应用在没有使用安全桌面的情况下提示提升。默认为启用|
|localSecurityOptionsUseAdminApprovalMode|Boolean|定义内置管理员帐户是使用管理员审批模式还是运行具有完全管理员权限的所有应用。默认为启用|
|localSecurityOptionsUseAdminApprovalModeForAdministrators|Boolean|定义是否启用管理员审批模式以及所有 UAC 策略设置，默认为启用|
|localSecurityOptionsInformationShownOnLockScreen|[localSecurityOptionsInformationShownOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|配置在会话锁定时显示的用户信息。 如果未配置，将显示显示名称、域和用户名。 可能的值是：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。|
|localSecurityOptionsInformationDisplayedOnLockScreen|[localSecurityOptionsInformationDisplayedOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|配置在会话锁定时显示的用户信息。 如果未配置，将显示显示名称、域和用户名。 可能的值是：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。|
|localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees|Boolean|此安全性设置确定 SMB 客户端是否尝试协商 SMB 数据包签名。|
|localSecurityOptionsClientDigitallySignCommunicationsAlways|Boolean|此安全性设置确定 SMB 客户端组件是否需要数据包签名。|
|localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers|Boolean|如果启用此安全性设置，则允许服务器消息阻止 (SMB) 重定向程序向在身份验证期间不支持密码加密的非 Microsoft SMB 服务器发送纯文本密码。|
|localSecurityOptionsDisableServerDigitallySignCommunicationsAlways|Boolean|此安全性设置确定 SMB 服务器组件是否需要数据包签名。|
|localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees|Boolean|此安全性设置确定 SMB 服务器是否与请求它的客户端协商 SMB 数据包签名。|
|localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares|Boolean|默认情况下，此安全设置限制匿名访问共享和通过管道访问可匿名访问的命名管道和可匿名访问的共享的设置|
|localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts|Boolean|此安全性设置确定将为与计算机的匿名连接授予哪些附加权限。|
|localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares|Boolean|此安全设置确定是否允许匿名用户执行某些活动，例如枚举域帐户和网络共享的名称。|
|localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange|Boolean|此安全设置确定是否在下次更改密码时存储 LAN 管理器 (LM) 存储新密码的哈希值。 默认情况下不存储它。|
|localSecurityOptionsSmartCardRemovalBehavior|[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|此安全设置确定从智能卡读卡器中删除登录用户的智能卡时会发生什么情况。 可能的值是：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。|
|defenderSecurityCenterDisableAppBrowserUI|Boolean|用于禁止显示应用和浏览器保护区域。|
|defenderSecurityCenterDisableFamilyUI|Boolean|用于禁止显示家庭选项区域。|
|defenderSecurityCenterDisableHealthUI|Boolean|用于禁止显示设备性能和运行状况区域。|
|defenderSecurityCenterDisableNetworkUI|Boolean|用于禁止显示防火墙和网络保护区域。|
|defenderSecurityCenterDisableVirusUI|Boolean|用于禁止显示病毒和威胁防护区域。|
|defenderSecurityCenterDisableAccountUI|Boolean|用于禁止显示帐户保护区域。|
|defenderSecurityCenterDisableClearTpmUI|Boolean|用于禁用"清除 TPM"按钮的显示。|
|defenderSecurityCenterDisableHardwareUI|Boolean|用于禁止显示硬件保护区域。|
|defenderSecurityCenterDisableNotificationAreaUI|Boolean|用于禁用通知区域控件的显示。 用户需要注销并登录或重新启动计算机，此设置才能生效。|
|defenderSecurityCenterDisableRansomwareUI|Boolean|用于禁止显示勒索软件保护区域。 |
|defenderSecurityCenterDisableSecureBootUI|Boolean|用于在"设备安全性"下禁用安全启动区域显示。|
|defenderSecurityCenterDisableTroubleshootingUI|Boolean|用于在"设备安全性"下禁止显示安全过程疑难解答。|
|defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI|Boolean|用于在检测到易受攻击的固件时禁用更新 TPM 固件的显示。|
|defenderSecurityCenterOrganizationDisplayName|String|向用户显示的公司名称。|
|defenderSecurityCenterHelpEmail|String|向用户显示的电子邮件地址。|
|defenderSecurityCenterHelpPhone|String|向用户Skype的电话号码或 ID。|
|defenderSecurityCenterHelpURL|String|向用户显示的帮助门户 URL。|
|defenderSecurityCenterNotificationsFromApp|[defenderSecurityCenterNotificationsFromAppType](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|从应用的显示区域显示的通知。 可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。|
|defenderSecurityCenterITContactDisplay|[defenderSecurityCenterITContactDisplayType](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|配置向最终用户显示 IT 联系人信息的地方。 可能的值是：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。|
|windowsDefenderTamperProtection|[windowsDefenderTamperProtectionOptions](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|配置 windows defender TamperProtection 设置。 可取值为：`notConfigured`、`enable`、`disable`。|
|firewallBlockStatefulFTP|Boolean|阻止到设备的有状态 FTP 连接|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。 这是一个时间段，在此之后安全关联将过期并被删除。 有效值为 300 至 3600|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|选择要使用的预共享密钥编码。 可取值为：`deviceDefault`、`none`、`utF8`。|
|firewallIPSecExemptionsNone|Boolean|将 IPSec 豁免配置为无免除|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码|
|firewallIPSecExemptionsAllowICMP|Boolean|配置 IPSec 免除项以允许 ICMP|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码|
|firewallIPSecExemptionsAllowDHCP|Boolean|配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|指定如何强制执行证书吊销列表。 可能的值是：`deviceDefault`、`none`、`attempt`、`require`。|
|firewallMergeKeyingModuleSettings|Boolean|如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|配置如何在隧道网关方案中应用数据包排队。 可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|配置域网络的防火墙配置文件设置|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|配置公用网络的防火墙配置文件设置|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|配置专用网络的防火墙配置文件设置|
|defenderAdobeReaderLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示 Adobe Reader 创建子进程的行为的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderAttackSurfaceReductionExcludedPaths|String 集合|要从攻击面减少规则中排除的 exe 文件和文件夹的列表|
|defenderOfficeAppsOtherProcessInjectionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示注入其他Office的应用程序的行为的值。 可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。|
|defenderOfficeAppsOtherProcessInjection|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示注入其他Office的应用程序的行为的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderOfficeCommunicationAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示创建子进程Office通信应用程序（包括 Microsoft Outlook）的行为的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderOfficeAppsExecutableContentCreationOrLaunchType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示应用程序/宏Office或启动可执行内容的行为的值。 可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。|
|defenderOfficeAppsExecutableContentCreationOrLaunch|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示应用程序/宏Office或启动可执行内容的行为的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderOfficeAppsLaunchChildProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示应用程序启动Office进程的行为的值。 可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。|
|defenderOfficeAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示应用程序启动Office进程的行为的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderOfficeMacroCodeAllowWin32ImportsType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示 Win32 从宏代码中从宏代码导入Office。 可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。|
|defenderOfficeMacroCodeAllowWin32Imports|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示 Win32 从宏代码中从宏代码导入Office。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderScriptObfuscatedMacroCodeType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示模糊化 js/vbs/ps/macro 代码行为的值。 可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。|
|defenderScriptObfuscatedMacroCode|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示模糊化 js/vbs/ps/macro 代码行为的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderScriptDownloadedPayloadExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示 js/vbs 执行从 Internet 下载的有效负载的行为的值。 可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。|
|defenderScriptDownloadedPayloadExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示 js/vbs 执行从 Internet 下载的有效负载的行为的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderPreventCredentialStealingType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示是否允许从本地安全Windows窃取凭据的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderProcessCreationType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示对源自 PSExec 和 WMI 命令的进程创建的响应的值。 可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。|
|defenderProcessCreation|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示对源自 PSExec 和 WMI 命令的进程创建的响应的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderUntrustedUSBProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示对从 USB 运行的不受信任的和未签名进程的响应的值。 可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。|
|defenderUntrustedUSBProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示对从 USB 运行的不受信任的和未签名进程的响应的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderUntrustedExecutableType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示对不符合普遍程度、年龄或受信任列表条件的可执行文件的响应的值。 可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。|
|defenderUntrustedExecutable|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示对不符合普遍程度、年龄或受信任列表条件的可执行文件的响应的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderEmailContentExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示执行可执行内容 (exe、dll、ps、js、vbs 等) 应从电子邮件 (webmail/mail-client) 。 可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。|
|defenderEmailContentExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示执行可执行内容 (exe、dll、ps、js、vbs 等) 应从电子邮件 (webmail/mail-client) 。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderAdvancedRansomewareProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示对勒索软件使用高级保护的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderGuardMyFoldersType|[folderProtectionType](../resources/intune-deviceconfig-folderprotectiontype.md)|指示受保护文件夹行为的值。 可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification`。|
|defenderGuardedFoldersAllowedAppPaths|String 集合|允许访问受保护文件夹的 exe 路径列表|
|defenderAdditionalGuardedFolders|String 集合|要添加到受保护文件夹列表的文件夹路径列表|
|defenderNetworkProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|指示 NetworkProtection 行为的值。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderExploitProtectionXml|Binary|包含有关 Exploit Protection 详细信息的 xml 内容。|
|defenderExploitProtectionXmlFileName|String|从中获取 DefenderExploitProtectionXml 的文件的名称。|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|指示是否阻止用户覆盖 Exploit Protection 设置。|
|defenderBlockPersistenceThroughWmiType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|指示通过 WMI 事件订阅阻止持久性的行为的值。 可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|使管理员能够选择在设备上允许哪些类型的应用。 可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。|
|deviceGuardLocalSystemAuthorityCredentialGuardSettings|[deviceGuardLocalSystemAuthorityCredentialGuardType](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|启用基于安全启动和虚拟化的安全性的平台安全级别时启用 Credential Guard。 可能的值是：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`、`disable`。|
|deviceGuardEnableVirtualizationBasedSecurity|Boolean|启用基于虚拟化的安全性 (VBS) 。|
|deviceGuardEnableSecureBootWithDMA|Boolean|此属性将在 2019 年 5 月弃用，并替换为属性 DeviceGuardSecureBootWithDMA。 指定下次重启时是否启用平台安全级别。|
|deviceGuardSecureBootWithDMA|[secureBootWithDMAType](../resources/intune-deviceconfig-securebootwithdmatype.md)|指定下次重启时是否启用平台安全级别。 可取值为：`notConfigured`、`withoutDMA`、`withDMA`。|
|deviceGuardLaunchSystemGuard|[enablement](../resources/intune-shared-enablement.md)|允许 IT 管理员配置 System Guard 的启动。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|smartScreenEnableInShell|Boolean|允许 IT 管理员配置适用于 Windows 的 SmartScreen。|
|smartScreenBlockOverrideForFiles|Boolean|允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。|
|applicationGuardEnabled|Boolean|启用 Windows Defender 应用程序防护|
|applicationGuardEnabledOptions|[applicationGuardEnabledOptions](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|为Windows Defender 应用程序防护版本启用Windows版本。 可能的值是：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。|
|applicationGuardBlockFileTransfer|[applicationGuardBlockFileTransferType](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|阻止剪贴板传输图像文件、文本文件或两者都不传输。 可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。|
|applicationGuardBlockNonEnterpriseContent|Boolean|阻止企业站点加载非企业内容，例如第三方插件|
|applicationGuardAllowPersistence|Boolean|允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据|
|applicationGuardForceAuditing|Boolean|强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）|
|applicationGuardBlockClipboardSharing|[applicationGuardBlockClipboardSharingType](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。 可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。|
|applicationGuardAllowPrintToPDF|Boolean|允许从容器打印为 PDF 格式|
|applicationGuardAllowPrintToXPS|Boolean|允许从容器打印为 XPS 格式|
|applicationGuardAllowPrintToLocalPrinters|Boolean|允许从容器打印到本地打印机|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|允许从容器打印到网络打印机|
|applicationGuardAllowVirtualGPU|布尔值|允许应用程序防护使用虚拟 GPU|
|applicationGuardAllowFileSaveOnHost|Boolean|允许用户从应用程序防护容器中的边缘下载文件并将其保存在主机文件系统上|
|applicationGuardAllowCameraMicrophoneRedirection|Boolean|获取或设置设备Microsoft Defender 应用程序防护应用程序是否可以访问设备的相机和麦克风。|
|applicationGuardCertificateThumbprints|String collection|允许与容器共享某些设备级别的根Microsoft Defender 应用程序防护证书。|
|bitLockerAllowStandardUserEncryption|Boolean|允许管理员允许标准用户在加入 Azure AD 期间启用订阅。|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|允许管理员禁用对用户计算机上其他磁盘加密的警告提示。|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|允许管理员要求使用 BitLocker 开启加密功能。 此策略仅适用于移动 SKU。|
|bitLockerEncryptDevice|Boolean|允许管理员要求使用 BitLocker 开启加密功能。|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|BitLocker 系统驱动器策略。|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|BitLocker 固定驱动器策略。|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|BitLocker 可移动驱动器策略。|
|bitLockerRecoveryPasswordRotation|[bitLockerRecoveryPasswordRotationType](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|此设置通过使用 bootmgr 或 WinRE (操作系统驱动器恢复后启动客户端驱动的恢复密码) 。 可能的值是：`notConfigured`、`disabled`、`enabledForAzureAd`、`enabledForAzureAdAndHybrid`。|
|defenderDisableScanArchiveFiles|Boolean|允许或禁止扫描存档。|
|defenderAllowScanArchiveFiles|Boolean|允许或禁止扫描存档。|
|defenderDisableBehaviorMonitoring|Boolean|允许或禁止Windows Defender监视功能。|
|defenderAllowBehaviorMonitoring|Boolean|允许或禁止Windows Defender监视功能。|
|defenderDisableCloudProtection|Boolean|为了最好地保护你的电脑，Windows Defender向 Microsoft 发送有关它所找到的任何问题的信息。 Microsoft 将分析该信息，了解有关影响您和其他客户的问题的更多信息，并提供改进的解决方案。|
|defenderAllowCloudProtection|Boolean|为了最好地保护你的电脑，Windows Defender向 Microsoft 发送有关它所找到的任何问题的信息。 Microsoft 将分析该信息，了解有关影响您和其他客户的问题的更多信息，并提供改进的解决方案。|
|defenderEnableScanIncomingMail|Boolean|允许或禁止扫描电子邮件。|
|defenderEnableScanMappedNetworkDrivesDuringFullScan|Boolean|允许或禁止对映射的网络驱动器进行完全扫描。|
|defenderDisableScanRemovableDrivesDuringFullScan|Boolean|允许或禁止对可移动驱动器进行完全扫描。 在快速扫描期间，仍可扫描可移动驱动器。|
|defenderAllowScanRemovableDrivesDuringFullScan|Boolean|允许或禁止对可移动驱动器进行完全扫描。 在快速扫描期间，仍可扫描可移动驱动器。|
|defenderDisableScanDownloads|布尔值|允许或禁止Windows Defender IOAVP 保护功能。|
|defenderAllowScanDownloads|Boolean|允许或禁止Windows Defender IOAVP 保护功能。|
|defenderDisableIntrusionPreventionSystem|布尔值|允许或禁止Windows Defender入侵防护功能。|
|defenderAllowIntrusionPreventionSystem|Boolean|允许或禁止Windows Defender入侵防护功能。|
|defenderDisableOnAccessProtection|Boolean|允许或禁止Windows Defender On Access Protection 功能。|
|defenderAllowOnAccessProtection|Boolean|允许或禁止Windows Defender On Access Protection 功能。|
|defenderDisableRealTimeMonitoring|Boolean|允许或禁止Windows Defender实时监视功能。|
|defenderAllowRealTimeMonitoring|Boolean|允许或禁止Windows Defender实时监视功能。|
|defenderDisableScanNetworkFiles|Boolean|允许或禁止扫描网络文件。|
|defenderAllowScanNetworkFiles|Boolean|允许或禁止扫描网络文件。|
|defenderDisableScanScriptsLoadedInInternetExplorer|Boolean|允许或禁止Windows Defender脚本扫描功能。|
|defenderAllowScanScriptsLoadedInInternetExplorer|Boolean|允许或禁止Windows Defender脚本扫描功能。|
|defenderBlockEndUserAccess|Boolean|允许或禁止用户访问 Windows Defender UI。 如果不允许，还将Windows Defender所有通知。|
|defenderAllowEndUserAccess|Boolean|允许或禁止用户访问 Windows Defender UI。 如果不允许，还将Windows Defender所有通知。|
|defenderScanMaxCpuPercentage|Int32|表示服务器扫描的平均 CPU 负载Windows Defender百 (百分比) 。 默认值为 50。 有效值为 0 至 100|
|defenderCheckForSignaturesBeforeRunningScan|Boolean|此策略设置允许你在运行扫描之前管理是否检查新的病毒定义和间谍软件定义。|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|已添加到Windows 10版本 1709 中。 此策略设置确定Windows Defender 防病毒和扫描可疑文件时的主动性。 值类型为整数。 此功能需要启用"加入 Microsoft MAPS"设置才能运行。 可能的值是：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。|
|defenderCloudExtendedTimeoutInSeconds|Int32|已添加到Windows 10版本 1709 中。 此功能允许Windows Defender 防病毒可疑文件最多阻止 60 秒，并扫描它在云中以确保其安全。 值类型为整数，范围为 0 - 50。 此功能依赖于必须全部启用的其他三个 MAPS 设置："配置'首次看到时阻止'功能;"加入 Microsoft MAPS";"需要进一步分析时发送文件示例"。 有效值为 0 至 50|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|时间段 (，) 隔离项目将存储在系统上的天数。 有效值为 0 至 90|
|defenderDisableCatchupFullScan|Boolean|此策略设置允许你为计划的完整扫描配置跟进扫描。 跟进扫描是因错过定期计划扫描而启动的扫描。 通常，这些计划扫描会丢失，因为计算机在计划时间已关闭。|
|defenderDisableCatchupQuickScan|Boolean|此策略设置允许你配置计划快速扫描的捕获扫描。 跟进扫描是因错过定期计划扫描而启动的扫描。 通常，这些计划扫描会丢失，因为计算机在计划时间已关闭。|
|defenderEnableLowCpuPriority|Boolean|此策略设置允许你为计划扫描启用或禁用低 CPU 优先级。|
|defenderFileExtensionsToExclude|String 集合|要从扫描和实时保护中排除的文件扩展名。|
|defenderFilesAndFoldersToExclude|String 集合|要从扫描和实时保护中排除的文件和文件夹。|
|defenderProcessesToExclude|String 集合|要从扫描和实时保护中排除的进程。|
|defenderPotentiallyUnwantedAppAction|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|已添加到 Windows 10 版本 1607 中。 指定对 PUA 中可能不需要的应用程序 (级别) 。 Windows Defender下载可能不需要的软件或尝试在计算机上安装自身时发出警报。 可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。|
|defenderScanDirection|[defenderRealtimeScanDirection](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|控制应监视哪些文件集。 可取值为：`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|选择是执行快速扫描还是完全扫描。 可能的值是：`userDefined`、`disabled`、`quick`、`full`。|
|defenderScheduledQuickScanTime|TimeOfDay|选择运行快速扫描Windows Defender的时间。 例如，值 0=12：00AM、值 60=1：00AM、值 120=2：00 等，最多为值 1380=11：00PM。 默认值为 120|
|defenderScheduledScanDay|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|选择运行扫描Windows Defender天。 可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan`。|
|defenderScheduledScanTime|TimeOfDay|选择一天中应运行Windows Defender的时间。|
|defenderSignatureUpdateIntervalInHours|Int32|指定 (检查签名的时间间隔) 以小时为单位，因此将按照间隔设置新签名的检查，而不是使用 ScheduleDay 和 ScheduleTime。 有效值为 0 至 24|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|在发送数据时检查用户Windows Defender级别。 可能的值是：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|允许管理员指定任何有效的威胁严重性级别和要采取的相应默认操作 ID。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
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
  "defenderBlockPersistenceThroughWmiType": "String",
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
  "applicationGuardAllowCameraMicrophoneRedirection": true,
  "applicationGuardCertificateThumbprints": [
    "String"
  ],
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



