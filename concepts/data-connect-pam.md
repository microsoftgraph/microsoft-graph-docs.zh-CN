---
title: Microsoft Graph 数据连接与 Privileged Access Management 的集成
description: Microsoft Graph 数据连接依赖于 Privileged Access Management 来允许 Office 365 管理员批准数据移动请求。
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: b09effe96a0b6c04ee68a23016f464a8e0f9d9e0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629815"
---
# <a name="microsoft-graph-data-connect-integration-with-privileged-access-management"></a><span data-ttu-id="c31af-103">Microsoft Graph 数据连接与 Privileged Access Management 的集成</span><span class="sxs-lookup"><span data-stu-id="c31af-103">Microsoft Graph data connect integration with Privileged Access Management</span></span>

<span data-ttu-id="c31af-104">Microsoft Graph 数据连接依赖于 Privileged Access Management (PAM) 来允许 Office 365 管理员批准数据移动请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-104">Microsoft Graph data connect relies on Privileged Access Management (PAM) to allow Office 365 administrators to approve data movement requests.</span></span> <span data-ttu-id="c31af-105">数据连接管道必须由 Office 365 管理员在启用期间指定的数据访问请求审批者批准。</span><span class="sxs-lookup"><span data-stu-id="c31af-105">Data connect pipelines must be approved by a member of the data access request approver specified by the Office 365 administrator during enablement.</span></span> <span data-ttu-id="c31af-106">若要设置审批者组，请参阅[入门](/concepts/data-connect-get-started.md)。</span><span class="sxs-lookup"><span data-stu-id="c31af-106">To set up the approver group, see [Get started](/concepts/data-connect-get-started.md).</span></span>

<span data-ttu-id="c31af-107">当复制活动请求访问权限以提取 Office 365 数据时，系统会向审批者的每名成员发送审批请求电子邮件来通知他们。</span><span class="sxs-lookup"><span data-stu-id="c31af-107">Approval request emails will be sent to each member of the approver group to notify them when copy activities request access to extract Office 365 data.</span></span> <span data-ttu-id="c31af-108">审批者可以批准或拒绝这些请求，指定应从提取的数据中清理的用户组，或撤销以前批准的请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-108">Approvers can approve or deny these requests, specify a user group that should be scrubbed out of extracted data, or revoke a previously approved request.</span></span> <span data-ttu-id="c31af-109">审批持续有效时间为 6 个月，并且 Azure 数据工厂管道中的每次复制活动都需要一次审批。</span><span class="sxs-lookup"><span data-stu-id="c31af-109">Approvals persist for 6 months, and one approval is needed per copy activity in the Azure Data Factory pipeline.</span></span> 

<span data-ttu-id="c31af-110">每个请求将始终包含有关数据集和将提取其相关数据的用户的以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="c31af-110">Every request will always include the following details about the dataset and the users about whom data is being extracted:</span></span>

* <span data-ttu-id="c31af-111">**Requestor**：发出管道请求的用户。</span><span class="sxs-lookup"><span data-stu-id="c31af-111">**Requestor**: The user who requested the pipeline.</span></span>
* <span data-ttu-id="c31af-112">**Duration**：在获得批准的情况下，审批将持续有效的时长 。</span><span class="sxs-lookup"><span data-stu-id="c31af-112">**Duration**: If approved, how long the approval will persist.</span></span> <span data-ttu-id="c31af-113">始终为 4320 小时（6 个月）。</span><span class="sxs-lookup"><span data-stu-id="c31af-113">Always 4320 hours (6 months).</span></span>
* <span data-ttu-id="c31af-114">**Reason**：请求的原因，通常为“为组织安装的应用需要审批才能访问 Office 365 数据”。</span><span class="sxs-lookup"><span data-stu-id="c31af-114">**Reason**: Reason for the request, typically "An app installed for your organization requires approval for access to Office 365 Data."</span></span>
* <span data-ttu-id="c31af-115">**Requested at**：请求的日期时间。</span><span class="sxs-lookup"><span data-stu-id="c31af-115">**Requested at**: The DateTime of the request.</span></span>
* <span data-ttu-id="c31af-116">**Request id**：请求的 ID，用于审批目的。</span><span class="sxs-lookup"><span data-stu-id="c31af-116">**Request id**: The ID of the request, used for approval purposes.</span></span>
* <span data-ttu-id="c31af-117">**DataTable**：所提取的数据集（例如，已发送邮件）。</span><span class="sxs-lookup"><span data-stu-id="c31af-117">**DataTable**: The data set being extracted (for example, Sent Items).</span></span>
* <span data-ttu-id="c31af-118">**Columns**：从数据表中提取的列的列表（例如，SentDateTime）。</span><span class="sxs-lookup"><span data-stu-id="c31af-118">**Columns**: The list of columns being extracted from the data table (for example, SentDateTime).</span></span>
* <span data-ttu-id="c31af-119">**AllowedGroups**：管道针对其提取数据的一个或多个用户组。</span><span class="sxs-lookup"><span data-stu-id="c31af-119">**AllowedGroups**: The group or groups of users against whom the pipeline is extracting data.</span></span> <span data-ttu-id="c31af-120">如果组列表为空，则管道会请求访问租户内所有用户中的数据。</span><span class="sxs-lookup"><span data-stu-id="c31af-120">If the list of groups is empty, the pipeline is requesting access to data from all users in the tenant.</span></span>
* <span data-ttu-id="c31af-121">**User Scope Query**：用于筛选出用户的谓词。</span><span class="sxs-lookup"><span data-stu-id="c31af-121">**User Scope Query**: The predicate used to filter out users.</span></span> <span data-ttu-id="c31af-122">仅在请求针对租户中的所有用户时适用。</span><span class="sxs-lookup"><span data-stu-id="c31af-122">Only applies if the request is for all users in the tenant.</span></span> <span data-ttu-id="c31af-123">如果此项为空，则不应用筛选器。</span><span class="sxs-lookup"><span data-stu-id="c31af-123">If this is empty, no filter is applied.</span></span> 
* <span data-ttu-id="c31af-124">**OutputUri**：将在其中存储提取的数据的输出路径。</span><span class="sxs-lookup"><span data-stu-id="c31af-124">**OutputUri**: The output path in which the extracted data will be stored.</span></span>
* <span data-ttu-id="c31af-125">**SourceTenantId**：从中提取数据的租户 ID。</span><span class="sxs-lookup"><span data-stu-id="c31af-125">**SourceTenantId**: The tenant ID from which data is being extracted.</span></span>
* <span data-ttu-id="c31af-126">**InstallerIdentity**：应用安装程序的标识。</span><span class="sxs-lookup"><span data-stu-id="c31af-126">**InstallerIdentity**: The identity of the app installer.</span></span>

<span data-ttu-id="c31af-127">请求中的以下字段将仅在某些情况下可用：</span><span class="sxs-lookup"><span data-stu-id="c31af-127">The following fields in the request will be available only in some cases:</span></span>

* <span data-ttu-id="c31af-128">“Application Name”和“Marketplace URI”（仅适用于通过 Azure 应用商店安装的应用程序）。</span><span class="sxs-lookup"><span data-stu-id="c31af-128">Application Name and the Marketplace URI (available only for applications installed from the Azure marketplace).</span></span>
* <span data-ttu-id="c31af-129">应用程序隐私政策及服务条款的链接（仅在应用程序提供时可用）。</span><span class="sxs-lookup"><span data-stu-id="c31af-129">Links to the application's privacy policy and terms of service (available only if the application provides it).</span></span>
* <span data-ttu-id="c31af-130">应用程序实施的合规性策略，例如输出存储位置中的静态数据加密（仅在应用程序提供该策略，并且应用程序是从 Azure 应用市场中安装的情况下，此字段才可用）。</span><span class="sxs-lookup"><span data-stu-id="c31af-130">The compliance policies that the application enforces, such as data encryption at rest in the output storage location (available only if the application provides it and if the application is installed from the Azure marketplace).</span></span>
* <span data-ttu-id="c31af-131">Deny List - 可从提取的数据中清理的用户名。</span><span class="sxs-lookup"><span data-stu-id="c31af-131">Deny List - The user group that can be scrubbed out of the extracted data.</span></span> <span data-ttu-id="c31af-132">作为支持从提取的数据中清理隐私的数据集请求的一部分，此字段为空。</span><span class="sxs-lookup"><span data-stu-id="c31af-132">This field is empty as a part of the request for datasets that support privacy scrubbing of extracted data.</span></span> <span data-ttu-id="c31af-133">负责批准请求的审批者组的成员可在审批时填充该字段。</span><span class="sxs-lookup"><span data-stu-id="c31af-133">It can be populated by the member of the approver group who approves the request at approval time.</span></span> 

## <a name="approving-requests"></a><span data-ttu-id="c31af-134">审批请求</span><span class="sxs-lookup"><span data-stu-id="c31af-134">Approving requests</span></span>

<span data-ttu-id="c31af-135">数据连接管道必须由数据访问请求审批者组的成员批准。</span><span class="sxs-lookup"><span data-stu-id="c31af-135">Data connect pipelines must be approved by a member of a data access request approver group.</span></span> <span data-ttu-id="c31af-136">审批者可通过使用 Exchange Online PowerShell 模块或 PAM 用户体验批准、拒绝或撤销管道。</span><span class="sxs-lookup"><span data-stu-id="c31af-136">Approvers can approve, deny, or revoke pipelines by using the Exchange Online PowerShell module or the PAM user experience.</span></span>

### <a name="approving-denying-and-revoking-requests-by-using-powershell"></a><span data-ttu-id="c31af-137">通过使用 PowerShell 批准、拒绝和撤销请求</span><span class="sxs-lookup"><span data-stu-id="c31af-137">Approving, denying, and revoking requests by using PowerShell</span></span>

<span data-ttu-id="c31af-138">使用以下步骤，通过 Exchange Online PowerShell 模块与请求交互：</span><span class="sxs-lookup"><span data-stu-id="c31af-138">Use the following steps to interact with a request using the Exchange Online PowerShell module:</span></span>

1. <span data-ttu-id="c31af-139">安装 Exchange Online Powershell 模块。</span><span class="sxs-lookup"><span data-stu-id="c31af-139">Install the Exchange Online Powershell module.</span></span> <span data-ttu-id="c31af-140">有关安装说明，请参阅[使用多重身份验证连接到 Exchange Online PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="c31af-140">For more information, see [Connect to Exchange Online PowerShell using multi-factor authentication](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span></span>

2. <span data-ttu-id="c31af-141">使用多重身份验证 (MFA) 连接到 Exchange Online PowerShell。</span><span class="sxs-lookup"><span data-stu-id="c31af-141">Connect to Exchange Online PowerShell using multi-factor authentication</span></span> <span data-ttu-id="c31af-142">有关说明，请参阅[使用多重身份验证连接到 Exchange Online PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="c31af-142">For more information, see [Connect to Exchange Online PowerShell using multi-factor authentication](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span></span>
    ><span data-ttu-id="c31af-143">**注意**：在连接到 Exchange Online PowerShell 时，你无需为组织启用多重身份验证便可使用这些步骤。</span><span class="sxs-lookup"><span data-stu-id="c31af-143">**Note**: You do not need to enable multi-factor authentication for your organization to use these steps while connecting to Exchange Online PowerShell.</span></span> <span data-ttu-id="c31af-144">通过 MFA 进行连接会创建一个 OAuth 令牌，PAM 将使用该令牌来为请求签名。</span><span class="sxs-lookup"><span data-stu-id="c31af-144">Connecting with MFA creates an OAuth token that is used by PAM for signing your requests.</span></span>

3. <span data-ttu-id="c31af-145">使用你的帐户登录。</span><span class="sxs-lookup"><span data-stu-id="c31af-145">Sign in with your organizational account.</span></span> <span data-ttu-id="c31af-146">请注意，你必须是配置的数据访问审批者组的成员才能批准、拒绝或撤销请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-146">Note that you must be part of the configured data access approver group in order to be able to approve, deny, or revoke requests.</span></span> <span data-ttu-id="c31af-147">来宾用户无法批准请求，即使他们是审批者组的成员。</span><span class="sxs-lookup"><span data-stu-id="c31af-147">Guest users cannot approve requests, even if they are in the approver group.</span></span> 

   ```powershell
   Connect-EXOPSSession
   ```

4. <span data-ttu-id="c31af-148">查找所有待处理的请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-148">Find all pending requests.</span></span>
   ><span data-ttu-id="c31af-149">**注意：\*\*\*\*Identity** 属性中的值将用于标识以及批准或拒绝请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-149">**Note:** The value in the **Identity** property will be used to identify and approve or deny the request.</span></span> <span data-ttu-id="c31af-150">记下此值，并在 -RequestId 参数中使用。</span><span class="sxs-lookup"><span data-stu-id="c31af-150">Note this value and use it in the -RequestId parameter.</span></span> 

   ```powershell
   Get-ElevatedAccessRequest | ?{$_.RequestStatus -eq 'Pending'}
   ```

4. <span data-ttu-id="c31af-151">仔细查看你感兴趣的请求的 **context** 字段。</span><span class="sxs-lookup"><span data-stu-id="c31af-151">Take a closer look at the **context** field of the request you are interested in.</span></span> 
   ><span data-ttu-id="c31af-152">**注意：** 数据访问请求的 context 字段描述复制活动的参数和属性。</span><span class="sxs-lookup"><span data-stu-id="c31af-152">**Note:** The context field of the data access request describes the parameters and properties of the copy activity.</span></span>

   ```powershell
   (Get-ElevatedAccessRequest -RequestId $requestId).Context | ConvertFrom-Json
   ```

   <span data-ttu-id="c31af-153">你将收到类似于如下的响应。</span><span class="sxs-lookup"><span data-stu-id="c31af-153">You'll get a response that looks like the following.</span></span>

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

5. <span data-ttu-id="c31af-154">为 -RequestId 参数使用 **Identity** 的值来批准/拒绝请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-154">Approve/deny the request using the value for **Identity** for the -RequestId parameter.</span></span>

   ```powershell
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!"
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

<span data-ttu-id="c31af-155">你也可以使用拒绝列表来批准请求，以确保不包括某些用户的数据。</span><span class="sxs-lookup"><span data-stu-id="c31af-155">You can also approve the request with a deny list to ensure data from certain users is not included.</span></span> <span data-ttu-id="c31af-156">为此，你需要修改请求的上下文以添加要忽略的组的 `object Id`，然后批准请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-156">To do so, you need to modify the context of the request to add the `object Id` of the group that you want to omit and then approve the request.</span></span> 

   ```powershell
   $request = Get-ElevatedAccessRequest -RequestId
   $hash = $request.Context
   $hash["DenyList"] = <Object ID of denied user group>;
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!" -RequestContext $hash
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```
<span data-ttu-id="c31af-157">你也可以撤销以前批准的请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-157">You can also revoke requests that were previously approved.</span></span> <span data-ttu-id="c31af-158">与审批请求类似，**Identity** 的值是 -RequestId 参数中的必需值。</span><span class="sxs-lookup"><span data-stu-id="c31af-158">Similar to approving requests, the value for **Identity** is what is required in the -RequestId parameter.</span></span> 

   ```powershell 
   Revoke-ElevatedAccessAuthorization -Comment "Revoking this request!" -RequestId $requestId
   ```
   <span data-ttu-id="c31af-159">你将看到类似于如下的响应。</span><span class="sxs-lookup"><span data-stu-id="c31af-159">You'll see a response similar to the following.</span></span>
   
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

### <a name="approving-denying-and-revoking-requests-by-using-the-pam-user-experience"></a><span data-ttu-id="c31af-160">通过使用 PAM 用户体验批准、拒绝和撤销请求</span><span class="sxs-lookup"><span data-stu-id="c31af-160">Approving, denying, and revoking requests by using the PAM user experience</span></span>

<span data-ttu-id="c31af-161">使用以下步骤，通过 PAM Web 体验与请求交互：</span><span class="sxs-lookup"><span data-stu-id="c31af-161">Use the following steps to interact with a request using the PAM web experience:</span></span>

1. <span data-ttu-id="c31af-162">使用管理员凭据登录到 Office 365 管理门户，并转到“[Privileged Access Managment 审批用户体验](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess)”页面。</span><span class="sxs-lookup"><span data-stu-id="c31af-162">Sign in to the Office 365 admin portal using admin credentials and go to the [Privileged Access Managment approval user experience](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess) page.</span></span> <span data-ttu-id="c31af-163">这将显示所有访问请求（待处理请求/已批准请求/已过期请求/已拒绝请求）。</span><span class="sxs-lookup"><span data-stu-id="c31af-163">This will show you all the access requests (pending/approved/expired/denied).</span></span>

<span data-ttu-id="c31af-164">在生成的页面上，选择你感兴趣的请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-164">On the resulting page, select the request that you are interested in.</span></span> <span data-ttu-id="c31af-165">若要选择用于清理隐私的拒绝列表，请单击“**拒绝列表**”下拉列表，选择需要清理的组，然后选择“**批准**”。</span><span class="sxs-lookup"><span data-stu-id="c31af-165">To select deny list for privacy scrubbing, click the **DenyList** dropdown, select the group that needs to be scrubbed, and then select **Approve**.</span></span>

<span data-ttu-id="c31af-166">若要撤销以前批准的请求，请选择需要撤销的已批准请求，并选择“**撤销**”。</span><span class="sxs-lookup"><span data-stu-id="c31af-166">To revoke a previously approved request, select the approved request that needs to be revoked, and choose **Revoke**.</span></span> <span data-ttu-id="c31af-167">下一次使用该审批转移数据的尝试将失败。</span><span class="sxs-lookup"><span data-stu-id="c31af-167">The next attempt to move data using that approval will fail.</span></span> 

### <a name="approval-behavior"></a><span data-ttu-id="c31af-168">审批行为</span><span class="sxs-lookup"><span data-stu-id="c31af-168">Approval behavior</span></span>

<span data-ttu-id="c31af-169">数据连接审批请求有一些务必要注意的特殊性质：</span><span class="sxs-lookup"><span data-stu-id="c31af-169">Data conenct approval requests have particular characteristics that are important to be aware of:</span></span>

- <span data-ttu-id="c31af-170">审批请求基于 Azure 数据工厂、管道和复制活动名称。</span><span class="sxs-lookup"><span data-stu-id="c31af-170">Approval requests are based on the Azure Data Factory, pipeline and copy activity names.</span></span> <span data-ttu-id="c31af-171">每次复制活动运行时，都将验证 Office 365 管理员是否批准了复制活动的 Office 数据访问请求，并将依据审批的参数验证复制活动运行的重要参数。</span><span class="sxs-lookup"><span data-stu-id="c31af-171">Every copy activity run will verify that the Office 365 admin has approved the copy activity's request to access Office data, and will validate the important parameters of the copy activity run against the parameters of the approval.</span></span>
- <span data-ttu-id="c31af-172">在某些条件下，将会自动触发新审批请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-172">Under certain conditions, a new approval request will automatically be triggered.</span></span> <span data-ttu-id="c31af-173">数据连接审批者将必须批准新请求，然后复制活动才能访问 Office 365 数据。</span><span class="sxs-lookup"><span data-stu-id="c31af-173">A data connect approver will have to approve the new request before the copy activity can access Office 365 data.</span></span>
- <span data-ttu-id="c31af-174">如果复制活动运行的参数发生变化，则会触发一个新的审批请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-174">If the parameters of the copy activity run changes, a new approval request will be triggered.</span></span>
- <span data-ttu-id="c31af-175">如果数据工厂、管道或复制活动名称发生变化，则会触发一个新的审批请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-175">If the Data Factory, pipeline or copy activity names change, a new approval request will be triggered.</span></span>
- <span data-ttu-id="c31af-176">例如：如果复制活动正在访问的数据表或列集发生变化，则需要进行一次新审批。</span><span class="sxs-lookup"><span data-stu-id="c31af-176">For example: A new approval will be required if the data table or set of columns that the copy activity is accessing changes.</span></span>
- <span data-ttu-id="c31af-177">必须每隔 6 个月审批一次复制活动。</span><span class="sxs-lookup"><span data-stu-id="c31af-177">Copy activities will have to be approved once every 6 months.</span></span> <span data-ttu-id="c31af-178">如果原始审批是 6 个月前批准的，则会自动触发一个新审批请求。</span><span class="sxs-lookup"><span data-stu-id="c31af-178">If the original approval was approved 6 months ago, a new approval request will automatically be triggered.</span></span>
- <span data-ttu-id="c31af-179">如果 Office 365 数据访问审批者拒绝了审批请求或撤销了以前批准的请求，则复制活动将持续失败。</span><span class="sxs-lookup"><span data-stu-id="c31af-179">If an Office 365 Data Access approver has denied an approval request or revoked a previously approved request, the copy activity will fail continually.</span></span> <span data-ttu-id="c31af-180">你应与审批者协作，了解拒绝或撤销原因，并相应修复复制活动的参数。</span><span class="sxs-lookup"><span data-stu-id="c31af-180">You should work with the approver to understand the reason for the denial or revocation and fix the parameters of the copy activity accordingly.</span></span> <span data-ttu-id="c31af-181">将必须部署新的复制活动或更改现有复制活动的名称，以便触发新的审批请求进行审批。</span><span class="sxs-lookup"><span data-stu-id="c31af-181">A new copy activity will have to deployed, or the name of the existing copy activity will have to be changed in order to trigger a new approval request for approval.</span></span>
- <span data-ttu-id="c31af-182">除非 Office 365 数据访问审批者对请求采取行动，否则审批请求将在 24 小时内过期。</span><span class="sxs-lookup"><span data-stu-id="c31af-182">An approval request will expire in 24 hours unless an Office 365 data access approver acts on the request.</span></span> <span data-ttu-id="c31af-183">将每隔 24 小时提交一次新请求以供审批。</span><span class="sxs-lookup"><span data-stu-id="c31af-183">A new request will be submitted once every 24 hours for approval.</span></span> <span data-ttu-id="c31af-184">如果看到复制活动正在等待审批（处于“等待同意”阶段），请与 Office 365 数据访问审批者协作，使你的请求获得批准。</span><span class="sxs-lookup"><span data-stu-id="c31af-184">If you see your copy activity waiting for approval (in the Consent Pending stage), then work with Office 365 data access approvers to get your request approved.</span></span>

## <a name="privacy-scrubbing"></a><span data-ttu-id="c31af-185">隐私清理</span><span class="sxs-lookup"><span data-stu-id="c31af-185">Privacy scrubbing</span></span> 
<span data-ttu-id="c31af-186">负责审批请求的审批者组成员可指定将从提取的数据中清理其数据的用户组的名称。</span><span class="sxs-lookup"><span data-stu-id="c31af-186">The member of the approver group who approves the request can specify the name of one user group whose data would be scrubbed out of extracted data.</span></span> <span data-ttu-id="c31af-187">如果行包含与已拒绝组的成员对应的电子邮件地址，则会从提取的数据中清理这些行。</span><span class="sxs-lookup"><span data-stu-id="c31af-187">The rows containing email addresses corresponding to the members of the denied group will be scrubbed out of extracted data.</span></span> <span data-ttu-id="c31af-188">嵌套在已拒绝组中的组将展开，并且将只会清理用户。有关如何在审批期间通过 PowerShell 或 PAM UX 应用拒绝列表的详细信息，请参阅本主题的“审批请求”部分。</span><span class="sxs-lookup"><span data-stu-id="c31af-188">Groups nested within the denied group will be expanded and only users will be scrubbed out. Refer to the approving requests section of this topic for details on how to apply the deny list during approval, through either PowerShell or the PAM UX.</span></span> 

<span data-ttu-id="c31af-189">下表显示了将对其内容进行隐私清理检查的数据集和列的名称。</span><span class="sxs-lookup"><span data-stu-id="c31af-189">The following table shows the names of the datasets and the columns for which the contents are checked for privacy scrubbing.</span></span>

| <span data-ttu-id="c31af-190">数据集名称</span><span class="sxs-lookup"><span data-stu-id="c31af-190">Dataset name</span></span>                     | <span data-ttu-id="c31af-191">用于基于拒绝列表的清理的列</span><span class="sxs-lookup"><span data-stu-id="c31af-191">Columns used for deny list-based scrubbing</span></span>                                                  |
|---------------------------------------------------------------------|----------------------------------------------------------|
| <span data-ttu-id="c31af-192">**BasicDataSet_v0.Message_v0**</span><span class="sxs-lookup"><span data-stu-id="c31af-192">**BasicDataSet_v0.Message_v0**</span></span><br><span data-ttu-id="c31af-193">**BasicDataSet_v0.Message_v1**</span><span class="sxs-lookup"><span data-stu-id="c31af-193">**BasicDataSet_v0.Message_v1**</span></span>   | <span data-ttu-id="c31af-194">Sender、From、ToRecipients、CcRecipients、BccRecipients</span><span class="sxs-lookup"><span data-stu-id="c31af-194">Sender, From, ToRecipients, CcRecipients, BccRecipients</span></span>    |                                                                               
| <span data-ttu-id="c31af-195">**BasicDataSet_v0.SentItem_v0**</span><span class="sxs-lookup"><span data-stu-id="c31af-195">**BasicDataSet_v0.SentItem_v0**</span></span><br><span data-ttu-id="c31af-196">**BasicDataSet_v0.SentItem_v1**</span><span class="sxs-lookup"><span data-stu-id="c31af-196">**BasicDataSet_v0.SentItem_v1**</span></span>  | <span data-ttu-id="c31af-197">Sender、From、ToRecipients、CcRecipients、BccRecipients</span><span class="sxs-lookup"><span data-stu-id="c31af-197">Sender, From, ToRecipients, CcRecipients, BccRecipients</span></span>  |
| <span data-ttu-id="c31af-198">**BasicDataSet_v0.Event_v0**</span><span class="sxs-lookup"><span data-stu-id="c31af-198">**BasicDataSet_v0.Event_v0**</span></span><br><span data-ttu-id="c31af-199">**BasicDataSet_v0.Event_v1**</span><span class="sxs-lookup"><span data-stu-id="c31af-199">**BasicDataSet_v0.Event_v1**</span></span>     | <span data-ttu-id="c31af-200">Organizer、Attendees</span><span class="sxs-lookup"><span data-stu-id="c31af-200">Organizer, Attendees</span></span>                                        |
| <span data-ttu-id="c31af-201">**BasicDataSet_v0.Contact_v0**</span><span class="sxs-lookup"><span data-stu-id="c31af-201">**BasicDataSet_v0.Contact_v0**</span></span><br><span data-ttu-id="c31af-202">**BasicDataSet_v0.Contact_v1**</span><span class="sxs-lookup"><span data-stu-id="c31af-202">**BasicDataSet_v0.Contact_v1**</span></span>  | <span data-ttu-id="c31af-203">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="c31af-203">emailAddresses</span></span>                                            |
| <span data-ttu-id="c31af-204">**BasicDataSet_v0.CalendarView_v0**</span><span class="sxs-lookup"><span data-stu-id="c31af-204">**BasicDataSet_v0.CalendarView_v0**</span></span>                                | <span data-ttu-id="c31af-205">Organizer、Attendees</span><span class="sxs-lookup"><span data-stu-id="c31af-205">Organizer, Attendees</span></span>                                      |

## <a name="next-steps"></a><span data-ttu-id="c31af-206">后续步骤</span><span class="sxs-lookup"><span data-stu-id="c31af-206">Next Steps</span></span>

<span data-ttu-id="c31af-207">确保你的组织已通过完成[入门](/concepts/data-connect-get-started.md)中的步骤正确配置了 Privileged Access Management 以与 Microsoft Graph 数据结合使用。</span><span class="sxs-lookup"><span data-stu-id="c31af-207">Ensure your organization has Privileged Access Management configured correctly for usage with Microsoft Graph data by completing the steps in [Get started](/concepts/data-connect-get-started.md).</span></span>
