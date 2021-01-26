---
title: office365ActiveUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 057490d5e19a8e56a2e83047277292fbd0af4a16
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980687"
---
# <a name="office365activeuserdetail-resource-type"></a><span data-ttu-id="8c288-103">office365ActiveUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c288-103">office365ActiveUserDetail resource type</span></span>

<span data-ttu-id="8c288-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c288-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="8c288-105">属性</span><span class="sxs-lookup"><span data-stu-id="8c288-105">Properties</span></span>

| <span data-ttu-id="8c288-106">属性</span><span class="sxs-lookup"><span data-stu-id="8c288-106">Property</span></span>                          | <span data-ttu-id="8c288-107">类型</span><span class="sxs-lookup"><span data-stu-id="8c288-107">Type</span></span>              | <span data-ttu-id="8c288-108">说明</span><span class="sxs-lookup"><span data-stu-id="8c288-108">Description</span></span>                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| <span data-ttu-id="8c288-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8c288-109">reportRefreshDate</span></span>                 | <span data-ttu-id="8c288-110">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-110">Date</span></span>              | <span data-ttu-id="8c288-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="8c288-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8c288-112">userPrincipalName</span></span>                 | <span data-ttu-id="8c288-113">String</span><span class="sxs-lookup"><span data-stu-id="8c288-113">String</span></span>            | <span data-ttu-id="8c288-114">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="8c288-114">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="8c288-115">UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。</span><span class="sxs-lookup"><span data-stu-id="8c288-115">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="8c288-116">按照惯例，此名称应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="8c288-116">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="8c288-117">常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。</span><span class="sxs-lookup"><span data-stu-id="8c288-117">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="8c288-118">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="8c288-118">This property is required when a user is created.</span></span> |
| <span data-ttu-id="8c288-119">displayName</span><span class="sxs-lookup"><span data-stu-id="8c288-119">displayName</span></span>                       | <span data-ttu-id="8c288-120">String</span><span class="sxs-lookup"><span data-stu-id="8c288-120">String</span></span>            | <span data-ttu-id="8c288-121">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="8c288-121">The name displayed in the address book for the user.</span></span> <span data-ttu-id="8c288-122">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="8c288-122">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="8c288-123">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="8c288-123">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="8c288-124">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8c288-124">isDeleted</span></span>                         | <span data-ttu-id="8c288-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c288-125">Boolean</span></span>           | <span data-ttu-id="8c288-126">此用户是已删除还是软删除。</span><span class="sxs-lookup"><span data-stu-id="8c288-126">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="8c288-127">deletedDate</span><span class="sxs-lookup"><span data-stu-id="8c288-127">deletedDate</span></span>                       | <span data-ttu-id="8c288-128">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-128">Date</span></span>              | <span data-ttu-id="8c288-129">执行删除操作的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-129">The date when the delete operation happened.</span></span> <span data-ttu-id="8c288-130">当用户尚未删除时，默认值为"null"。</span><span class="sxs-lookup"><span data-stu-id="8c288-130">Default value is "null" when the user has not been deleted.</span></span> |
| <span data-ttu-id="8c288-131">hasExchangeLicense</span><span class="sxs-lookup"><span data-stu-id="8c288-131">hasExchangeLicense</span></span>                | <span data-ttu-id="8c288-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c288-132">Boolean</span></span>           | <span data-ttu-id="8c288-133">是否已为用户分配 Exchange 许可证。</span><span class="sxs-lookup"><span data-stu-id="8c288-133">Whether the user has been assigned an Exchange license.</span></span> |
| <span data-ttu-id="8c288-134">hasOneDriveLicense</span><span class="sxs-lookup"><span data-stu-id="8c288-134">hasOneDriveLicense</span></span>                | <span data-ttu-id="8c288-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c288-135">Boolean</span></span>           | <span data-ttu-id="8c288-136">是否已为用户分配 OneDrive 许可证。</span><span class="sxs-lookup"><span data-stu-id="8c288-136">Whether the user has been assigned a OneDrive license.</span></span> |
| <span data-ttu-id="8c288-137">hasSharePointLicense</span><span class="sxs-lookup"><span data-stu-id="8c288-137">hasSharePointLicense</span></span>              | <span data-ttu-id="8c288-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c288-138">Boolean</span></span>           | <span data-ttu-id="8c288-139">是否已为用户分配 SharePoint 许可证。</span><span class="sxs-lookup"><span data-stu-id="8c288-139">Whether the user has been assigned a SharePoint license.</span></span> |
| <span data-ttu-id="8c288-140">hasSkypeForBusinessLicense</span><span class="sxs-lookup"><span data-stu-id="8c288-140">hasSkypeForBusinessLicense</span></span>        | <span data-ttu-id="8c288-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c288-141">Boolean</span></span>           | <span data-ttu-id="8c288-142">是否已为用户分配 Skype For Business 许可证。</span><span class="sxs-lookup"><span data-stu-id="8c288-142">Whether the user has been assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="8c288-143">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="8c288-143">hasYammerLicense</span></span>                  | <span data-ttu-id="8c288-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c288-144">Boolean</span></span>           | <span data-ttu-id="8c288-145">是否已为用户分配 Yammer 许可证。</span><span class="sxs-lookup"><span data-stu-id="8c288-145">Whether the user has been assigned a Yammer license.</span></span> |
| <span data-ttu-id="8c288-146">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="8c288-146">hasTeamsLicense</span></span>                   | <span data-ttu-id="8c288-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c288-147">Boolean</span></span>           | <span data-ttu-id="8c288-148">是否已为用户分配 Teams 许可证。</span><span class="sxs-lookup"><span data-stu-id="8c288-148">Whether the user has been assigned a Teams license.</span></span> |
| <span data-ttu-id="8c288-149">exchangeLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8c288-149">exchangeLastActivityDate</span></span>          | <span data-ttu-id="8c288-150">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-150">Date</span></span>              | <span data-ttu-id="8c288-151">用户上次阅读或发送电子邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-151">The date when user last read or sent email.</span></span> |
| <span data-ttu-id="8c288-152">oneDriveLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8c288-152">oneDriveLastActivityDate</span></span>          | <span data-ttu-id="8c288-153">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-153">Date</span></span>              | <span data-ttu-id="8c288-154">用户上次查看或编辑文件、在内部或外部共享文件或同步文件的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-154">The date when user last viewed or edited files, shared files internally or externally, or synced files.</span></span> |
| <span data-ttu-id="8c288-155">sharePointLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8c288-155">sharePointLastActivityDate</span></span>        | <span data-ttu-id="8c288-156">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-156">Date</span></span>              | <span data-ttu-id="8c288-157">用户上次查看或编辑文件、在内部或外部共享文件、同步文件或查看 SharePoint 页面的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-157">The date when user last viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages.</span></span> |
| <span data-ttu-id="8c288-158">skypeForBusinessLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8c288-158">skypeForBusinessLastActivityDate</span></span>  | <span data-ttu-id="8c288-159">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-159">Date</span></span>              | <span data-ttu-id="8c288-160">用户上次组织或参与会议或加入对等会话的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-160">The date when user last organized or participated in conferences, or joined peer-to-peer sessions.</span></span> |
| <span data-ttu-id="8c288-161">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8c288-161">yammerLastActivityDate</span></span>            | <span data-ttu-id="8c288-162">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-162">Date</span></span>              | <span data-ttu-id="8c288-163">用户上次发布、阅读或喜欢的邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-163">The date when user last posted, read, or liked message.</span></span> |
| <span data-ttu-id="8c288-164">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8c288-164">teamsLastActivityDate</span></span>             | <span data-ttu-id="8c288-165">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-165">Date</span></span>              | <span data-ttu-id="8c288-166">用户上次在团队频道中发布消息、在私人聊天会话中发送消息或参与会议或通话的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-166">The date when user last posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls.</span></span> |
| <span data-ttu-id="8c288-167">exchangeLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8c288-167">exchangeLicenseAssignDate</span></span>         | <span data-ttu-id="8c288-168">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-168">Date</span></span>              | <span data-ttu-id="8c288-169">上次为用户分配 Exchange 许可证的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-169">The last date when the user was assigned an Exchange license.</span></span> |
| <span data-ttu-id="8c288-170">oneDriveLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8c288-170">oneDriveLicenseAssignDate</span></span>         | <span data-ttu-id="8c288-171">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-171">Date</span></span>              | <span data-ttu-id="8c288-172">上次向用户分配 OneDrive 许可证的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-172">The last date when the user was assigned a OneDrive license.</span></span> |
| <span data-ttu-id="8c288-173">sharePointLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8c288-173">sharePointLicenseAssignDate</span></span>       | <span data-ttu-id="8c288-174">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-174">Date</span></span>              | <span data-ttu-id="8c288-175">上次为用户分配 SharePoint 许可证的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-175">The last date when the user was assigned a SharePoint license.</span></span> |
| <span data-ttu-id="8c288-176">skypeForBusinessLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8c288-176">skypeForBusinessLicenseAssignDate</span></span> | <span data-ttu-id="8c288-177">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-177">Date</span></span>              | <span data-ttu-id="8c288-178">为用户分配 Skype For Business 许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-178">The last date when the user was assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="8c288-179">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8c288-179">yammerLicenseAssignDate</span></span>           | <span data-ttu-id="8c288-180">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-180">Date</span></span>              | <span data-ttu-id="8c288-181">上次为用户分配 Yammer 许可证的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-181">The last date when the user was assigned a Yammer license.</span></span> |
| <span data-ttu-id="8c288-182">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8c288-182">teamsLicenseAssignDate</span></span>            | <span data-ttu-id="8c288-183">日期</span><span class="sxs-lookup"><span data-stu-id="8c288-183">Date</span></span>              | <span data-ttu-id="8c288-184">上次向用户分配 Teams 许可证的日期。</span><span class="sxs-lookup"><span data-stu-id="8c288-184">The last date when the user was assigned a Teams license.</span></span> |
| <span data-ttu-id="8c288-185">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="8c288-185">assignedProducts</span></span>                  | <span data-ttu-id="8c288-186">String collection</span><span class="sxs-lookup"><span data-stu-id="8c288-186">String collection</span></span> | <span data-ttu-id="8c288-187">为用户分配的所有产品。</span><span class="sxs-lookup"><span data-stu-id="8c288-187">All the products assigned for the user.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8c288-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c288-188">JSON representation</span></span>

<span data-ttu-id="8c288-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c288-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "hasExchangeLicense": true, 
  "hasOneDriveLicense": true, 
  "hasSharePointLicense": true, 
  "hasSkypeForBusinessLicense": true, 
  "hasYammerLicense": true, 
  "hasTeamsLicense": true, 
  "exchangeLastActivityDate": "Date", 
  "oneDriveLastActivityDate": "Date", 
  "sharePointLastActivityDate": "Date", 
  "skypeForBusinessLastActivityDate": "Date", 
  "yammerLastActivityDate": "Date", 
  "teamsLastActivityDate": "Date", 
  "exchangeLicenseAssignDate": "Date", 
  "oneDriveLicenseAssignDate": "Date", 
  "sharePointLicenseAssignDate": "Date", 
  "skypeForBusinessLicenseAssignDate": "Date", 
  "yammerLicenseAssignDate": "Date", 
  "teamsLicenseAssignDate": "Date", 
  "assignedProducts": ["String"]
}
```


