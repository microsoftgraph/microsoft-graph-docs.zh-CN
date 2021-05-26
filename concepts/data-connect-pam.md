---
title: Microsoft Graph 数据连接与 Privileged Access Management 的集成
description: Microsoft Graph 数据连接依赖于 Privileged Access Management 来允许 Microsoft 365 管理员批准数据移动请求。
author: fercobo-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 3631b652c5e17c333548662b429a56ce3015f55b
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629320"
---
# <a name="microsoft-graph-data-connect-integration-with-privileged-access-management"></a><span data-ttu-id="2db78-103">Microsoft Graph 数据连接与 Privileged Access Management 的集成</span><span class="sxs-lookup"><span data-stu-id="2db78-103">Microsoft Graph Data Connect integration with Privileged Access Management</span></span>

<span data-ttu-id="2db78-104">Microsoft Graph 数据连接依赖于 Privileged Access Management (PAM) 来允许 Microsoft 365 管理员批准数据移动请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-104">Microsoft Graph Data Connect relies on Privileged Access Management (PAM) to allow Microsoft 365 administrators to approve data movement requests.</span></span> <span data-ttu-id="2db78-105">数据连接管道必须由 Microsoft 365 管理员在启用期间指定的数据访问请求审批者批准。</span><span class="sxs-lookup"><span data-stu-id="2db78-105">Data Connect pipelines must be approved by a member of the data access request approver specified by the Microsoft 365 administrator during enablement.</span></span> <span data-ttu-id="2db78-106">若要设置审批者组，请参阅[入门](data-connect-get-started.md)。</span><span class="sxs-lookup"><span data-stu-id="2db78-106">To set up the approver group, see [Get started](data-connect-get-started.md).</span></span>

<span data-ttu-id="2db78-107">当复制活动请求访问权限以提取 Microsoft 365 数据时，系统会向审批者的每名成员发送审批请求电子邮件来通知他们。</span><span class="sxs-lookup"><span data-stu-id="2db78-107">Approval request emails will be sent to each member of the approver group to notify them when copy activities request access to extract Microsoft 365 data.</span></span> <span data-ttu-id="2db78-108">审批者可以批准或拒绝这些请求，指定应从提取的数据中清理的用户组，或撤销以前批准的请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-108">Approvers can approve or deny these requests, specify a user group that should be scrubbed out of extracted data, or revoke a previously approved request.</span></span> <span data-ttu-id="2db78-109">审批持续时间为 6 个月，并且 Azure 数据工厂管道中的每次复制活动都需要进行审批。</span><span class="sxs-lookup"><span data-stu-id="2db78-109">Approvals persist for 6 months, and one approval is needed per copy activity in the Azure Data Factory pipeline.</span></span>

<span data-ttu-id="2db78-110">每个请求将始终包含以下详细信息，包括有关数据集和将提取其相关数据的用户：</span><span class="sxs-lookup"><span data-stu-id="2db78-110">Every request will always include the following details about the dataset and the users about whom data is being extracted:</span></span>

* <span data-ttu-id="2db78-111">**Requestor**：发出管道请求的用户。</span><span class="sxs-lookup"><span data-stu-id="2db78-111">**Requestor**: The user who requested the pipeline.</span></span>
* <span data-ttu-id="2db78-112">**Duration**：在获得批准的情况下，审批将持续有效的时长。</span><span class="sxs-lookup"><span data-stu-id="2db78-112">**Duration**: If approved, how long the approval will persist.</span></span> <span data-ttu-id="2db78-113">始终为 4320 小时（6 个月）。</span><span class="sxs-lookup"><span data-stu-id="2db78-113">Always 4320 hours (6 months).</span></span>
* <span data-ttu-id="2db78-114">**Reason**：请求的原因，通常为“组织安装的应用需要批准以访问 Office 365 数据”。</span><span class="sxs-lookup"><span data-stu-id="2db78-114">**Reason**: Reason for the request, typically "An app installed for your organization requires approval for access to Office 365 Data."</span></span>
* <span data-ttu-id="2db78-115">**Requested at**：请求的日期时间。</span><span class="sxs-lookup"><span data-stu-id="2db78-115">**Requested at**: The DateTime of the request.</span></span>
* <span data-ttu-id="2db78-116">**Request id**：请求的 ID，用于审批目的。</span><span class="sxs-lookup"><span data-stu-id="2db78-116">**Request id**: The ID of the request, used for approval purposes.</span></span>
* <span data-ttu-id="2db78-117">**DataTable**：所提取的数据集（例如，已发送邮件）。</span><span class="sxs-lookup"><span data-stu-id="2db78-117">**DataTable**: The data set being extracted (for example, Sent Items).</span></span>
* <span data-ttu-id="2db78-118">**Columns**：从数据表中提取的列的列表（例如，SentDateTime）。</span><span class="sxs-lookup"><span data-stu-id="2db78-118">**Columns**: The list of columns being extracted from the data table (for example, SentDateTime).</span></span>
* <span data-ttu-id="2db78-119">**AllowedGroups**：管道针对其提取数据的一个或多个用户组。</span><span class="sxs-lookup"><span data-stu-id="2db78-119">**AllowedGroups**: The group or groups of users against whom the pipeline is extracting data.</span></span> <span data-ttu-id="2db78-120">如果组列表为空，则管道会请求访问租户内所有用户中的数据。</span><span class="sxs-lookup"><span data-stu-id="2db78-120">If the list of groups is empty, the pipeline is requesting access to data from all users in the tenant.</span></span>
* <span data-ttu-id="2db78-121">**User Scope Query**：用于筛选出用户的谓词。</span><span class="sxs-lookup"><span data-stu-id="2db78-121">**User Scope Query**: The predicate used to filter out users.</span></span> <span data-ttu-id="2db78-122">仅在请求针对租户中的所有用户时适用。</span><span class="sxs-lookup"><span data-stu-id="2db78-122">Only applies if the request is for all users in the tenant.</span></span> <span data-ttu-id="2db78-123">如果此项为空，则不应用筛选器。</span><span class="sxs-lookup"><span data-stu-id="2db78-123">If this is empty, no filter is applied.</span></span>
* <span data-ttu-id="2db78-124">**OutputUri**：将存储提取数据的输出路径。</span><span class="sxs-lookup"><span data-stu-id="2db78-124">**OutputUri**: The output path in which the extracted data will be stored.</span></span>
* <span data-ttu-id="2db78-125">**SourceTenantId**：从中提取数据的租户 ID。</span><span class="sxs-lookup"><span data-stu-id="2db78-125">**SourceTenantId**: The tenant ID from which data is being extracted.</span></span>
* <span data-ttu-id="2db78-126">**InstallerIdentity**：应用安装程序的标识。</span><span class="sxs-lookup"><span data-stu-id="2db78-126">**InstallerIdentity**: The identity of the app installer.</span></span>

<span data-ttu-id="2db78-127">请求中的以下字段将仅在某些情况下可用：</span><span class="sxs-lookup"><span data-stu-id="2db78-127">The following fields in the request will be available only in some cases:</span></span>

* <span data-ttu-id="2db78-128">“Application Name”和“Marketplace URI”（仅适用于通过 Azure 应用商店安装的应用程序）。</span><span class="sxs-lookup"><span data-stu-id="2db78-128">Application Name and the Marketplace URI (available only for applications installed from the Azure marketplace).</span></span>
* <span data-ttu-id="2db78-129">应用程序隐私政策及服务条款的链接（仅在应用程序提供时可用）。</span><span class="sxs-lookup"><span data-stu-id="2db78-129">Links to the application's privacy policy and terms of service (available only if the application provides it).</span></span>
* <span data-ttu-id="2db78-130">应用程序实施的合规性策略，例如输出存储位置的静态数据加密（仅在应用程序提供该策略，并且应用程序是从 Azure 应用市场中安装的情况下可用）。</span><span class="sxs-lookup"><span data-stu-id="2db78-130">The compliance policies that the application enforces, such as data encryption at rest in the output storage location (available only if the application provides it and if the application is installed from the Azure marketplace).</span></span>
* <span data-ttu-id="2db78-131">拒绝列表 - 可从提取数据中清理的用户组。</span><span class="sxs-lookup"><span data-stu-id="2db78-131">Deny List - The user group that can be scrubbed out of the extracted data.</span></span> <span data-ttu-id="2db78-132">如果作为支持从提取数据中清理隐私的数据集请求的一部分，则此字段为空。</span><span class="sxs-lookup"><span data-stu-id="2db78-132">This field is empty as a part of the request for datasets that support privacy scrubbing of extracted data.</span></span> <span data-ttu-id="2db78-133">负责批准请求的审批者组的成员可在审批时填充该字段。</span><span class="sxs-lookup"><span data-stu-id="2db78-133">It can be populated by the member of the approver group who approves the request at approval time.</span></span>

## <a name="approving-requests"></a><span data-ttu-id="2db78-134">审批请求</span><span class="sxs-lookup"><span data-stu-id="2db78-134">Approving requests</span></span>

<span data-ttu-id="2db78-135">数据连接管道必须由数据访问请求审批者组的成员批准。</span><span class="sxs-lookup"><span data-stu-id="2db78-135">Data Connect pipelines must be approved by a member of a data access request approver group.</span></span> <span data-ttu-id="2db78-136">审批者可通过使用 Exchange Online PowerShell 模块或 PAM 用户体验批准、拒绝或撤销管道。</span><span class="sxs-lookup"><span data-stu-id="2db78-136">Approvers can approve, deny, or revoke pipelines by using the Exchange Online PowerShell module or the PAM user experience.</span></span>

### <a name="approving-denying-and-revoking-requests-by-using-powershell"></a><span data-ttu-id="2db78-137">通过使用 PowerShell 批准、拒绝和撤销请求</span><span class="sxs-lookup"><span data-stu-id="2db78-137">Approving, denying, and revoking requests by using PowerShell</span></span>

<span data-ttu-id="2db78-138">使用以下步骤，通过 Exchange Online PowerShell 模块与请求交互：</span><span class="sxs-lookup"><span data-stu-id="2db78-138">Use the following steps to interact with a request using the Exchange Online PowerShell module:</span></span>

1. <span data-ttu-id="2db78-139">安装 Exchange Online Powershell 模块。</span><span class="sxs-lookup"><span data-stu-id="2db78-139">Install the Exchange Online Powershell module.</span></span> <span data-ttu-id="2db78-140">有关安装说明，请参阅[使用多重身份验证连接到 Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="2db78-140">For installation instructions, see [Connect to Exchange Online PowerShell using multi-factor authentication](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span></span>

2. <span data-ttu-id="2db78-141">使用多重身份验证 (MFA) 连接到 Exchange Online PowerShell。</span><span class="sxs-lookup"><span data-stu-id="2db78-141">Connect to Exchange Online Powershell using multi-factor authentication (MFA).</span></span> <span data-ttu-id="2db78-142">有关说明，请参阅[使用多重身份验证连接到 Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="2db78-142">For instructions, see [Connect to Exchange Online PowerShell using multi-factor authentication](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span></span>
    > [!NOTE]
    > <span data-ttu-id="2db78-143">**注意**：在连接到 Exchange Online PowerShell 时，你无需为组织启用多重身份验证便可使用这些步骤。</span><span class="sxs-lookup"><span data-stu-id="2db78-143">**Note**: You do not need to enable multi-factor authentication for your organization to use these steps while connecting to Exchange Online PowerShell.</span></span> <span data-ttu-id="2db78-144">使用 MFA 进行连接会创建一个 OAuth 令牌，PAM 将使用该令牌来为请求签名。</span><span class="sxs-lookup"><span data-stu-id="2db78-144">Connecting with MFA creates an OAuth token that is used by PAM for signing your requests.</span></span>

3. <span data-ttu-id="2db78-145">使用你的帐户登录。</span><span class="sxs-lookup"><span data-stu-id="2db78-145">Sign in with your account.</span></span> <span data-ttu-id="2db78-146">请注意，你必须是配置的数据访问审批者组的成员才能批准、拒绝或撤销请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-146">Note that you must be part of the configured data access approver group in order to be able to approve, deny, or revoke requests.</span></span> <span data-ttu-id="2db78-147">来宾用户无法批准请求，即使他们是审批者组的成员。</span><span class="sxs-lookup"><span data-stu-id="2db78-147">Guest users cannot approve requests, even if they are in the approver group.</span></span>

   ```powershell
   Connect-EXOPSSession
   ```

4. <span data-ttu-id="2db78-148">查找所有待处理的请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-148">Find all pending requests.</span></span>
   > [!NOTE]
   > <span data-ttu-id="2db78-149">**Identity** 属性中的值将用于标识以及批准或拒绝请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-149">The value in the **Identity** property will be used to identify and approve or deny the request.</span></span> <span data-ttu-id="2db78-150">记下此值，并在 -RequestId 参数中使用。</span><span class="sxs-lookup"><span data-stu-id="2db78-150">Note this value and use it in the -RequestId parameter.</span></span>

   ```powershell
   Get-ElevatedAccessRequest | ?{$_.RequestStatus -eq 'Pending'}
   ```

5. <span data-ttu-id="2db78-151">仔细查看你感兴趣的请求的 **context** 字段。</span><span class="sxs-lookup"><span data-stu-id="2db78-151">Take a closer look at the **context** field of the request you are interested in.</span></span>
   ><span data-ttu-id="2db78-152">**注意：** 数据访问请求的 context 字段描述复制活动的参数和属性。</span><span class="sxs-lookup"><span data-stu-id="2db78-152">**Note:** The context field of the data access request describes the parameters and properties of the copy activity.</span></span>

   ```powershell
   Get-ElevatedAccessRequest -RequestId $requestId).Context | ConvertFrom-Json
   ```

   <span data-ttu-id="2db78-153">你将收到如下所示的响应。</span><span class="sxs-lookup"><span data-stu-id="2db78-153">You'll get a response that looks like the following.</span></span>

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

6. <span data-ttu-id="2db78-154">为 -RequestId 参数使用 **Identity** 的值来批准/拒绝请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-154">Approve/deny the request using the value for **Identity** for the -RequestId parameter.</span></span>

   ```powershell
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!"
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

<span data-ttu-id="2db78-155">你也可以使用拒绝列表来批准请求，以确保不包括某些用户的数据。</span><span class="sxs-lookup"><span data-stu-id="2db78-155">You can also approve the request with a deny list to ensure data from certain users is not included.</span></span> <span data-ttu-id="2db78-156">为此，你需要修改请求的上下文以添加要忽略的组的 `object Id`，然后批准请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-156">To do so, you need to modify the context of the request to add the `object Id` of the group that you want to omit and then approve the request.</span></span>

   ```powershell
   $request = Get-ElevatedAccessRequest -RequestId
   $hash = $request.Context
   $hash["DenyList"] = <Object ID of denied user group>;
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!" -RequestContext $hash
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

<span data-ttu-id="2db78-157">你也可以撤销以前批准的请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-157">You can also revoke requests that were previously approved.</span></span> <span data-ttu-id="2db78-158">与审批请求类似，**Identity** 的值是 -RequestId 参数中的必需值。</span><span class="sxs-lookup"><span data-stu-id="2db78-158">Similar to approving requests, the value for **Identity** is what is required in the -RequestId parameter.</span></span>

   ```powershell
   Revoke-ElevatedAccessAuthorization -Comment "Revoking this request!" -RequestId $requestId
   ```

   <span data-ttu-id="2db78-159">你将看到如下所示的响应。</span><span class="sxs-lookup"><span data-stu-id="2db78-159">You'll see a response similar to the following.</span></span>

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

### <a name="approving-denying-and-revoking-requests-by-using-the-pam-user-experience"></a><span data-ttu-id="2db78-160">通过使用 PAM 用户体验批准、拒绝和撤销请求</span><span class="sxs-lookup"><span data-stu-id="2db78-160">Approving, denying, and revoking requests by using the PAM user experience</span></span>

<span data-ttu-id="2db78-161">使用以下步骤，通过 PAM Web 体验与请求交互：</span><span class="sxs-lookup"><span data-stu-id="2db78-161">Use the following steps to interact with a request using the PAM web experience:</span></span>

1. <span data-ttu-id="2db78-162">使用管理员凭据登录到 Microsoft 365 管理门户，并转到“[Privileged Access Managment 审批用户体验](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess)”页面。</span><span class="sxs-lookup"><span data-stu-id="2db78-162">Sign in to the Microsoft 365 admin portal using admin credentials and go to the [Privileged Access Managment approval user experience](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess) page.</span></span> <span data-ttu-id="2db78-163">这将显示所有访问请求（待处理请求/已批准请求/已过期请求/已拒绝请求）。</span><span class="sxs-lookup"><span data-stu-id="2db78-163">This will show you all the access requests (pending/approved/expired/denied).</span></span>

2. <span data-ttu-id="2db78-164">在生成的页面上，选择你感兴趣的请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-164">On the resulting page, select the request that you're interested in.</span></span> <span data-ttu-id="2db78-165">若要选择用于清理隐私的拒绝列表，请单击“**拒绝列表**”下拉列表，选择需要清理的组，然后选择“**批准**”。</span><span class="sxs-lookup"><span data-stu-id="2db78-165">To select a deny list for privacy scrubbing, click the **DenyList** dropdown, select the group that needs to be scrubbed, and then select **Approve**.</span></span>

3. <span data-ttu-id="2db78-166">若要撤销以前批准的请求，请选择需要撤销的已批准请求，并选择“**撤销**”。</span><span class="sxs-lookup"><span data-stu-id="2db78-166">To revoke a previously approved request, select the approved request that needs to be revoked, and choose **Revoke**.</span></span> <span data-ttu-id="2db78-167">下一次使用该审批转移数据的尝试将失败。</span><span class="sxs-lookup"><span data-stu-id="2db78-167">The next attempt to move data using that approval will fail.</span></span>

### <a name="approval-behavior"></a><span data-ttu-id="2db78-168">审批行为</span><span class="sxs-lookup"><span data-stu-id="2db78-168">Approval behavior</span></span>

<span data-ttu-id="2db78-169">数据连接审批请求有一些务必要注意的特性：</span><span class="sxs-lookup"><span data-stu-id="2db78-169">Data Connect approval requests have particular characteristics that are important to be aware of:</span></span>

* <span data-ttu-id="2db78-p118">审批请求基于 Azure 数据工厂、管道和复制活动名称。每次复制活动运行时，都将验证 Microsoft 365 管理员是否批准了复制活动关于访问 Office 数据的请求，并将依据审批的参数验证复制活动运行的重要参数。</span><span class="sxs-lookup"><span data-stu-id="2db78-p118">Approval requests are based on the Azure Data Factory, pipeline and copy activity names. Every copy activity run will verify that the Microsoft 365 admin has approved the copy activity's request to access Office data, and will validate the important parameters of the copy activity run against the parameters of the approval.</span></span>
* <span data-ttu-id="2db78-172">在某些条件下，将会自动触发新审批请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-172">Under certain conditions, a new approval request will automatically be triggered.</span></span> <span data-ttu-id="2db78-173">数据连接审批者将必须批准新请求，然后复制活动才能访问 Microsoft 365 数据。</span><span class="sxs-lookup"><span data-stu-id="2db78-173">A Data Connect approver will have to approve the new request before the copy activity can access Microsoft 365 data.</span></span>
* <span data-ttu-id="2db78-174">如果复制活动运行的参数发生变化，则会触发一个新的审批请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-174">If the parameters of the copy activity run changes, a new approval request will be triggered.</span></span>
* <span data-ttu-id="2db78-175">如果数据工厂、管道或复制活动名称发生变化，则会触发一个新的审批请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-175">If the Data Factory, pipeline or copy activity names change, a new approval request will be triggered.</span></span>
* <span data-ttu-id="2db78-176">例如：如果复制活动正在访问的数据表或列集发生变化，则需要进行一次新审批。</span><span class="sxs-lookup"><span data-stu-id="2db78-176">For example: A new approval will be required if the data table or set of columns that the copy activity is accessing changes.</span></span>
* <span data-ttu-id="2db78-177">必须每隔 6 个月审批一次复制活动。</span><span class="sxs-lookup"><span data-stu-id="2db78-177">Copy activities will have to be approved once every 6 months.</span></span> <span data-ttu-id="2db78-178">如果原始审批是 6 个月前批准的，则会自动触发一个新审批请求。</span><span class="sxs-lookup"><span data-stu-id="2db78-178">If the original approval was approved 6 months ago, a new approval request will automatically be triggered.</span></span>
* <span data-ttu-id="2db78-179">如果 Microsoft 365 数据访问审批者拒绝了审批请求或撤销了以前批准的请求，则复制活动将持续失败。</span><span class="sxs-lookup"><span data-stu-id="2db78-179">If a Microsoft 365 Data Access approver has denied an approval request or revoked a previously approved request, the copy activity will fail continually.</span></span> <span data-ttu-id="2db78-180">你应与审批者协作，了解拒绝或撤销原因，并相应修复复制活动的参数。</span><span class="sxs-lookup"><span data-stu-id="2db78-180">You should work with the approver to understand the reason for the denial or revocation and fix the parameters of the copy activity accordingly.</span></span> <span data-ttu-id="2db78-181">必须部署新的复制活动或更改现有复制活动的名称，以便触发新的审批请求进行审批。</span><span class="sxs-lookup"><span data-stu-id="2db78-181">A new copy activity will have to deployed, or the name of the existing copy activity will have to be changed in order to trigger a new approval request for approval.</span></span>
* <span data-ttu-id="2db78-182">如果 Microsoft 365 数据访问审批者未处理请求，则审批请求将在 24 小时内过期。</span><span class="sxs-lookup"><span data-stu-id="2db78-182">An approval request will expire in 24 hours unless a Microsoft 365 data access approver acts on the request.</span></span> <span data-ttu-id="2db78-183">将每隔 24 小时提交一次新请求以供审批。</span><span class="sxs-lookup"><span data-stu-id="2db78-183">A new request will be submitted once every 24 hours for approval.</span></span> <span data-ttu-id="2db78-184">如果看到复制活动正在等待审批（处于“等待同意”阶段），请与 Microsoft 365 数据访问审批者协作，使你的请求获得批准。</span><span class="sxs-lookup"><span data-stu-id="2db78-184">If you see your copy activity waiting for approval (in the Consent Pending stage), then work with Microsoft 365 data access approvers to get your request approved.</span></span>

## <a name="privacy-scrubbing"></a><span data-ttu-id="2db78-185">隐私清理</span><span class="sxs-lookup"><span data-stu-id="2db78-185">Privacy scrubbing</span></span>

<span data-ttu-id="2db78-186">负责审批请求的审批者组成员可指定将从提取的数据中清理其数据的用户组名称。</span><span class="sxs-lookup"><span data-stu-id="2db78-186">The member of the approver group who approves the request can specify the name of one user group whose data would be scrubbed out of extracted data.</span></span> <span data-ttu-id="2db78-187">如果行包含与已拒绝组的成员对应的电子邮件地址，则会从提取的数据中清理这些行。</span><span class="sxs-lookup"><span data-stu-id="2db78-187">The rows containing email addresses corresponding to the members of the denied group will be scrubbed out of extracted data.</span></span> <span data-ttu-id="2db78-188">嵌套在已拒绝组中的组将展开，只会清理用户。有关如何在审批期间通过 PowerShell 或 PAM UX 应用拒绝列表的详细信息，请参阅本主题的“审批请求”部分。</span><span class="sxs-lookup"><span data-stu-id="2db78-188">Groups nested within the denied group will be expanded and only users will be scrubbed out. Refer to the approving requests section of this topic for details on how to apply the deny list during approval, through either PowerShell or the PAM UX.</span></span>

<span data-ttu-id="2db78-189">下表显示了将对其内容进行隐私清理检查的数据集和列的名称。</span><span class="sxs-lookup"><span data-stu-id="2db78-189">The following table shows the names of the datasets and the columns for which the contents are checked for privacy scrubbing.</span></span>

| <span data-ttu-id="2db78-190">数据集名称</span><span class="sxs-lookup"><span data-stu-id="2db78-190">Dataset name</span></span>                                                       | <span data-ttu-id="2db78-191">用于基于拒绝列表进行清理的列</span><span class="sxs-lookup"><span data-stu-id="2db78-191">Columns used for deny list-based scrubbing</span></span>              |
| ------------------------------------------------------------------ | ------------------------------------------------------- |
| <span data-ttu-id="2db78-192">**BasicDataSet_v0.Message_v0**</span><span class="sxs-lookup"><span data-stu-id="2db78-192">**BasicDataSet_v0.Message_v0**</span></span><br><span data-ttu-id="2db78-193">**BasicDataSet_v0.Message_v1**</span><span class="sxs-lookup"><span data-stu-id="2db78-193">**BasicDataSet_v0.Message_v1**</span></span>   | <span data-ttu-id="2db78-194">Sender、From、ToRecipients、CcRecipients、BccRecipients</span><span class="sxs-lookup"><span data-stu-id="2db78-194">Sender, From, ToRecipients, CcRecipients, BccRecipients</span></span> |
| <span data-ttu-id="2db78-195">**BasicDataSet_v0.SentItem_v0**</span><span class="sxs-lookup"><span data-stu-id="2db78-195">**BasicDataSet_v0.SentItem_v0**</span></span><br><span data-ttu-id="2db78-196">**BasicDataSet_v0.SentItem_v1**</span><span class="sxs-lookup"><span data-stu-id="2db78-196">**BasicDataSet_v0.SentItem_v1**</span></span> | <span data-ttu-id="2db78-197">Sender、From、ToRecipients、CcRecipients、BccRecipients</span><span class="sxs-lookup"><span data-stu-id="2db78-197">Sender, From, ToRecipients, CcRecipients, BccRecipients</span></span> |
| <span data-ttu-id="2db78-198">**BasicDataSet_v0.Event_v0**</span><span class="sxs-lookup"><span data-stu-id="2db78-198">**BasicDataSet_v0.Event_v0**</span></span><br><span data-ttu-id="2db78-199">**BasicDataSet_v0.Event_v1**</span><span class="sxs-lookup"><span data-stu-id="2db78-199">**BasicDataSet_v0.Event_v1**</span></span>       | <span data-ttu-id="2db78-200">Organizer、Attendees</span><span class="sxs-lookup"><span data-stu-id="2db78-200">Organizer, Attendees</span></span>                                    |
| <span data-ttu-id="2db78-201">**BasicDataSet_v0.Contact_v0**</span><span class="sxs-lookup"><span data-stu-id="2db78-201">**BasicDataSet_v0.Contact_v0**</span></span><br><span data-ttu-id="2db78-202">**BasicDataSet_v0.Contact_v1**</span><span class="sxs-lookup"><span data-stu-id="2db78-202">**BasicDataSet_v0.Contact_v1**</span></span>   | <span data-ttu-id="2db78-203">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="2db78-203">EmailAddresses</span></span>                                          |
| <span data-ttu-id="2db78-204">**BasicDataSet_v0.CalendarView_v0**</span><span class="sxs-lookup"><span data-stu-id="2db78-204">**BasicDataSet_v0.CalendarView_v0**</span></span>                                | <span data-ttu-id="2db78-205">Organizer、Attendees</span><span class="sxs-lookup"><span data-stu-id="2db78-205">Organizer, Attendees</span></span>                                    |

## <a name="see-also"></a><span data-ttu-id="2db78-206">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2db78-206">See also</span></span>

- [<span data-ttu-id="2db78-207">数据连接常见问题解答</span><span class="sxs-lookup"><span data-stu-id="2db78-207">Data Connect frequently asked questions</span></span>](data-connect-faq.md)
