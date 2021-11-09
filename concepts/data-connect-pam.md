---
title: Microsoft Graph 数据连接与 Privileged Access Management 的集成
description: Microsoft Graph 数据连接依赖于 Privileged Access Management 来允许 Microsoft 365 管理员批准数据移动请求。
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: f7e68ceb0a58d03818d838566fb8d8421018a97e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695179"
---
# <a name="microsoft-graph-data-connect-integration-with-privileged-access-management"></a>Microsoft Graph 数据连接与 Privileged Access Management 的集成

Microsoft Graph 数据连接依赖于 Privileged Access Management (PAM) 来允许 Microsoft 365 管理员批准数据移动请求。 数据连接管道必须由 Microsoft 365 管理员在启用期间指定的数据访问请求审批者批准。 若要设置审批者组，请参阅[设置 Microsoft 365 租户并启用 Microsoft Graph 数据连接](https://docs.microsoft.com/graph/data-connect-quickstart?tabs=Microsoft365&tutorial-step=1)。

当复制活动请求访问权限以提取 Microsoft 365 数据时，系统会向审批者的每名成员发送审批请求电子邮件来通知他们。 审批者可以批准或拒绝这些请求，指定应从提取的数据中清理的用户组，或撤销以前批准的请求。 审批持续时间为 6 个月，并且 Azure 数据工厂管道中的每次复制活动都需要进行审批。

每个请求将始终包含以下详细信息，包括有关数据集和将提取其相关数据的用户：

* **Requestor**：发出管道请求的用户。
* **Duration**：在获得批准的情况下，审批将持续有效的时长。 始终为 4320 小时（6 个月）。
* **Reason**：请求的原因，通常为“组织安装的应用需要批准以访问 Office 365 数据”。
* **Requested at**：请求的日期时间。
* **Request id**：请求的 ID，用于审批目的。
* **DataTable**：所提取的数据集（例如，已发送邮件）。
* **Columns**：从数据表中提取的列的列表（例如，SentDateTime）。
* **AllowedGroups**：管道针对其提取数据的一个或多个用户组。 如果组列表为空，则管道会请求访问租户内所有用户中的数据。
* **User Scope Query**：用于筛选出用户的谓词。 仅在请求针对租户中的所有用户时适用。 如果此项为空，则不应用筛选器。
* **OutputUri**：将存储提取数据的输出路径。
* **SourceTenantId**：从中提取数据的租户 ID。
* **InstallerIdentity**：应用安装程序的标识。

请求中的以下字段将仅在某些情况下可用：

* “Application Name”和“Marketplace URI”（仅适用于通过 Azure 应用商店安装的应用程序）。
* 应用程序隐私政策及服务条款的链接（仅在应用程序提供时可用）。
* 应用程序实施的合规性策略，例如输出存储位置的静态数据加密（仅在应用程序提供该策略，并且应用程序是从 Azure 应用市场中安装的情况下可用）。
* 拒绝列表 - 可从提取数据中清理的用户组。 如果作为支持从提取数据中清理隐私的数据集请求的一部分，则此字段为空。 负责批准请求的审批者组的成员可在审批时填充该字段。

## <a name="approving-requests"></a>审批请求

数据连接管道必须由数据访问请求审批者组的成员批准。 审批者可通过使用 Exchange Online PowerShell 模块或 PAM 用户体验批准、拒绝或撤销管道。

### <a name="approving-denying-and-revoking-requests-by-using-powershell"></a>通过使用 PowerShell 批准、拒绝和撤销请求

使用以下步骤，通过 Exchange Online PowerShell 模块与请求交互：

1. 安装 Exchange Online Powershell 模块。 有关安装说明，请参阅[使用多重身份验证连接到 Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps)。

2. 使用多重身份验证 (MFA) 连接到 Exchange Online PowerShell。 有关说明，请参阅[使用多重身份验证连接到 Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps)。
    > [!NOTE]
    > **注意**：在连接到 Exchange Online PowerShell 时，你无需为组织启用多重身份验证便可使用这些步骤。 使用 MFA 进行连接会创建一个 OAuth 令牌，PAM 将使用该令牌来为请求签名。

3. 使用你的帐户登录。 请注意，你必须是配置的数据访问审批者组的成员才能批准、拒绝或撤销请求。 来宾用户无法批准请求，即使他们是审批者组的成员。

   ```powershell
   Connect-EXOPSSession
   ```

4. 查找所有待处理的请求。
   > [!NOTE]
   > **Identity** 属性中的值将用于标识以及批准或拒绝请求。 记下此值，并在 -RequestId 参数中使用。

   ```powershell
   Get-ElevatedAccessRequest | ?{$_.RequestStatus -eq 'Pending'}
   ```

5. 仔细查看你感兴趣的请求的 **context** 字段。
   >**注意：** 数据访问请求的 context 字段描述复制活动的参数和属性。

   ```powershell
   Get-ElevatedAccessRequest -RequestId $requestId).Context | ConvertFrom-Json
   ```

   你将收到如下所示的响应。

   ```powershell
   Key                          Value
   ---                          -----
   ApplicationName
   ComplianceStatus             [{"Timestamp":"2018-05-02T18:29:21.5705664Z","RequirementName":"adlsEncryption","PolicyComplianceState":"Compliant","Violations":0},{"Timestamp":"2018-05-02T...
   ApplicationMarketPlaceUri
   OutputUri                    adl://myadlserumvrroyspmq.azuredatalakestore.net/targetFolder/Event
   ApplicationPrivacyPolicyUri  http://www.wkw.com/privacy
   ApplicationTermsOfServiceUri http://www.wkw.com/tos
   InstallerIdentity            a89885c3-4b0e-499e-86ed-14d7ed9147c2@942229f8-4656-4fb0-828b-e938dad4019a
   SourceTenantId               942229f8-4656-4fb0-828b-e938dad4019a
   UserScopeQuery               tenant in (942229f8-4656-4fb0-828b-e938dad4019a)
   ApplicationId
   DataTable                    Calendar Events
   DestinationTenantId          942229f8-4656-4fb0-828b-e938dad4019a
   Columns                      Subject:string, HasAttachments:bool, End:DateTime, Start:DateTime, ResponseStatus:string, Organizer:Object, Attendees:string, Importance:string, Sensitivity:...
   ```

6. 为 -RequestId 参数使用 **Identity** 的值来批准/拒绝请求。

   ```powershell
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!"
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

你也可以使用拒绝列表来批准请求，以确保不包括某些用户的数据。 为此，你需要修改请求的上下文以添加要忽略的组的 `object Id`，然后批准请求。

   ```powershell
   $request = Get-ElevatedAccessRequest -RequestId
   $hash = $request.Context
   $hash["DenyList"] = <Object ID of denied user group>;
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!" -RequestContext $hash
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

你也可以撤销以前批准的请求。 与审批请求类似，**Identity** 的值是 -RequestId 参数中的必需值。

   ```powershell
   Revoke-ElevatedAccessAuthorization -Comment "Revoking this request!" -RequestId $requestId
   ```

   你将看到如下所示的响应。

   ```powershell
   AuthorizedBy          : user@tenant.onmicrosoft.com
   Type                  : Task
   AuthorizedAccess      : Data Access Request
   StartTimeUtc          : 7/24/2018 6:02:42 PM
   EndTimeUtc            : 10/22/2018 6:02:42 PM
   Revoked               : True
   RevocationDateTimeUtc : 7/24/2018 9:12:55 PM
   RevokedBy             : NAMPR00A001.prod.outlook.com/Microsoft Exchange Hosted  Organizations/tenant.onmicrosoft.com/user
   RevocationComment     : Revoking this request!
   Identity              : bda75607-0d87-43cb-bdf1-284b18446b34
   DateCreatedUtc        : 1/1/0001 12:00:00 AM
   DateUpdatedUtc        : 7/24/2018 9:12:55 PM
   ```

### <a name="approving-denying-and-revoking-requests-by-using-the-pam-user-experience"></a>通过使用 PAM 用户体验批准、拒绝和撤销请求

使用以下步骤，通过 PAM Web 体验与请求交互：

1. 使用管理员凭据登录到 Microsoft 365 管理门户，并转到“[Privileged Access Managment 审批用户体验](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess)”页面。 这将显示所有访问请求（待处理请求/已批准请求/已过期请求/已拒绝请求）。

2. 在生成的页面上，选择你感兴趣的请求。 若要选择用于清理隐私的拒绝列表，请单击“**拒绝列表**”下拉列表，选择需要清理的组，然后选择“**批准**”。

3. 若要撤销以前批准的请求，请选择需要撤销的已批准请求，并选择“**撤销**”。 下一次使用该审批转移数据的尝试将失败。

### <a name="approval-behavior"></a>审批行为

数据连接审批请求有一些务必要注意的特性：

* 审批请求基于 Azure 数据工厂、管道和复制活动名称。每次复制活动运行时，都将验证 Microsoft 365 管理员是否批准了复制活动关于访问 Office 数据的请求，并将依据审批的参数验证复制活动运行的重要参数。
* 在某些条件下，将会自动触发新审批请求。 数据连接审批者将必须批准新请求，然后复制活动才能访问 Microsoft 365 数据。
* 如果复制活动运行的参数发生变化，则会触发一个新的审批请求。
* 如果数据工厂、管道或复制活动名称发生变化，则会触发一个新的审批请求。
* 例如：如果复制活动正在访问的数据表或列集发生变化，则需要进行一次新审批。
* 必须每隔 6 个月审批一次复制活动。 如果原始审批是 6 个月前批准的，则会自动触发一个新审批请求。
* 如果 Microsoft 365 数据访问审批者拒绝了审批请求或撤销了以前批准的请求，则复制活动将持续失败。 你应与审批者协作，了解拒绝或撤销原因，并相应修复复制活动的参数。 必须部署新的复制活动或更改现有复制活动的名称，以便触发新的审批请求进行审批。
* 如果 Microsoft 365 数据访问审批者未处理请求，则审批请求将在 24 小时内过期。 将每隔 24 小时提交一次新请求以供审批。 如果看到复制活动正在等待审批（处于“等待同意”阶段），请与 Microsoft 365 数据访问审批者协作，使你的请求获得批准。

## <a name="privacy-scrubbing"></a>隐私清理

负责审批请求的审批者组成员可指定将从提取的数据中清理其数据的用户组名称。 如果行包含与已拒绝组的成员对应的电子邮件地址，则会从提取的数据中清理这些行。 嵌套在已拒绝组中的组将展开，只会清理用户。有关如何在审批期间通过 PowerShell 或 PAM UX 应用拒绝列表的详细信息，请参阅本主题的“审批请求”部分。

下表显示了将对其内容进行隐私清理检查的数据集和列的名称。

| 数据集名称                                                       | 用于基于拒绝列表进行清理的列              |
| ------------------------------------------------------------------ | ------------------------------------------------------- |
| **BasicDataSet_v0.Message_v0**<br>**BasicDataSet_v0.Message_v1**   | Sender、From、ToRecipients、CcRecipients、BccRecipients |
| **BasicDataSet_v0.SentItem_v0**<br>**BasicDataSet_v0.SentItem_v1** | Sender、From、ToRecipients、CcRecipients、BccRecipients |
| **BasicDataSet_v0.Event_v0**<br>**BasicDataSet_v0.Event_v1**       | Organizer、Attendees                                    |
| **BasicDataSet_v0.Contact_v0**<br>**BasicDataSet_v0.Contact_v1**   | EmailAddresses                                          |
| **BasicDataSet_v0.CalendarView_v0**                                | Organizer、Attendees                                    |

## <a name="see-also"></a>另请参阅

- [数据连接常见问题解答](data-connect-faq.md)
