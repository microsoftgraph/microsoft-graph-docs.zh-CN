---
title: office365ActiveUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 7027d581e9dfd883a7dca6f91d3a1d56184097ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522461"
---
# <a name="office365activeuserdetail-resource-type"></a><span data-ttu-id="8286f-103">office365ActiveUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="8286f-103">office365ActiveUserDetail resource type</span></span>

<span data-ttu-id="8286f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8286f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="8286f-105">属性</span><span class="sxs-lookup"><span data-stu-id="8286f-105">Properties</span></span>

| <span data-ttu-id="8286f-106">属性</span><span class="sxs-lookup"><span data-stu-id="8286f-106">Property</span></span>                          | <span data-ttu-id="8286f-107">类型</span><span class="sxs-lookup"><span data-stu-id="8286f-107">Type</span></span>              | <span data-ttu-id="8286f-108">说明</span><span class="sxs-lookup"><span data-stu-id="8286f-108">Description</span></span>                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| <span data-ttu-id="8286f-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8286f-109">reportRefreshDate</span></span>                 | <span data-ttu-id="8286f-110">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-110">Date</span></span>              | <span data-ttu-id="8286f-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="8286f-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8286f-112">userPrincipalName</span></span>                 | <span data-ttu-id="8286f-113">String</span><span class="sxs-lookup"><span data-stu-id="8286f-113">String</span></span>            | <span data-ttu-id="8286f-114">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="8286f-114">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="8286f-115">UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。</span><span class="sxs-lookup"><span data-stu-id="8286f-115">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="8286f-116">按照惯例，此名称应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="8286f-116">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="8286f-117">常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。</span><span class="sxs-lookup"><span data-stu-id="8286f-117">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="8286f-118">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="8286f-118">This property is required when a user is created.</span></span> |
| <span data-ttu-id="8286f-119">displayName</span><span class="sxs-lookup"><span data-stu-id="8286f-119">displayName</span></span>                       | <span data-ttu-id="8286f-120">String</span><span class="sxs-lookup"><span data-stu-id="8286f-120">String</span></span>            | <span data-ttu-id="8286f-121">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="8286f-121">The name displayed in the address book for the user.</span></span> <span data-ttu-id="8286f-122">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="8286f-122">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="8286f-123">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="8286f-123">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="8286f-124">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8286f-124">isDeleted</span></span>                         | <span data-ttu-id="8286f-125">布尔</span><span class="sxs-lookup"><span data-stu-id="8286f-125">Boolean</span></span>           | <span data-ttu-id="8286f-126">此用户是否已被删除或软删除。</span><span class="sxs-lookup"><span data-stu-id="8286f-126">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="8286f-127">deletedDate</span><span class="sxs-lookup"><span data-stu-id="8286f-127">deletedDate</span></span>                       | <span data-ttu-id="8286f-128">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-128">Date</span></span>              | <span data-ttu-id="8286f-129">删除操作发生的日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-129">The date when the delete operation happened.</span></span> <span data-ttu-id="8286f-130">当用户未被删除时，默认值为 "null"。</span><span class="sxs-lookup"><span data-stu-id="8286f-130">Default value is "null" when the user has not been deleted.</span></span> |
| <span data-ttu-id="8286f-131">hasExchangeLicense</span><span class="sxs-lookup"><span data-stu-id="8286f-131">hasExchangeLicense</span></span>                | <span data-ttu-id="8286f-132">布尔</span><span class="sxs-lookup"><span data-stu-id="8286f-132">Boolean</span></span>           | <span data-ttu-id="8286f-133">是否已为用户分配了 Exchange 许可证。</span><span class="sxs-lookup"><span data-stu-id="8286f-133">Whether the user has been assigned an Exchange license.</span></span> |
| <span data-ttu-id="8286f-134">hasOneDriveLicense</span><span class="sxs-lookup"><span data-stu-id="8286f-134">hasOneDriveLicense</span></span>                | <span data-ttu-id="8286f-135">布尔</span><span class="sxs-lookup"><span data-stu-id="8286f-135">Boolean</span></span>           | <span data-ttu-id="8286f-136">是否已为用户分配 OneDrive 许可证。</span><span class="sxs-lookup"><span data-stu-id="8286f-136">Whether the user has been assigned a OneDrive license.</span></span> |
| <span data-ttu-id="8286f-137">hasSharePointLicense</span><span class="sxs-lookup"><span data-stu-id="8286f-137">hasSharePointLicense</span></span>              | <span data-ttu-id="8286f-138">布尔</span><span class="sxs-lookup"><span data-stu-id="8286f-138">Boolean</span></span>           | <span data-ttu-id="8286f-139">是否已为用户分配 SharePoint 许可证。</span><span class="sxs-lookup"><span data-stu-id="8286f-139">Whether the user has been assigned a SharePoint license.</span></span> |
| <span data-ttu-id="8286f-140">hasSkypeForBusinessLicense</span><span class="sxs-lookup"><span data-stu-id="8286f-140">hasSkypeForBusinessLicense</span></span>        | <span data-ttu-id="8286f-141">布尔</span><span class="sxs-lookup"><span data-stu-id="8286f-141">Boolean</span></span>           | <span data-ttu-id="8286f-142">是否已为用户分配 Skype For Business 许可证。</span><span class="sxs-lookup"><span data-stu-id="8286f-142">Whether the user has been assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="8286f-143">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="8286f-143">hasYammerLicense</span></span>                  | <span data-ttu-id="8286f-144">布尔</span><span class="sxs-lookup"><span data-stu-id="8286f-144">Boolean</span></span>           | <span data-ttu-id="8286f-145">是否为用户分配了 Yammer 许可证。</span><span class="sxs-lookup"><span data-stu-id="8286f-145">Whether the user has been assigned a Yammer license.</span></span> |
| <span data-ttu-id="8286f-146">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="8286f-146">hasTeamsLicense</span></span>                   | <span data-ttu-id="8286f-147">布尔</span><span class="sxs-lookup"><span data-stu-id="8286f-147">Boolean</span></span>           | <span data-ttu-id="8286f-148">是否已向用户分配团队许可证。</span><span class="sxs-lookup"><span data-stu-id="8286f-148">Whether the user has been assigned a Teams license.</span></span> |
| <span data-ttu-id="8286f-149">exchangeLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8286f-149">exchangeLastActivityDate</span></span>          | <span data-ttu-id="8286f-150">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-150">Date</span></span>              | <span data-ttu-id="8286f-151">用户最后一次阅读或发送电子邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-151">The date when user last read or sent email.</span></span> |
| <span data-ttu-id="8286f-152">oneDriveLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8286f-152">oneDriveLastActivityDate</span></span>          | <span data-ttu-id="8286f-153">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-153">Date</span></span>              | <span data-ttu-id="8286f-154">用户上次查看或编辑文件、内部或外部共享文件或同步文件的日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-154">The date when user last viewed or edited files, shared files internally or externally, or synced files.</span></span> |
| <span data-ttu-id="8286f-155">sharePointLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8286f-155">sharePointLastActivityDate</span></span>        | <span data-ttu-id="8286f-156">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-156">Date</span></span>              | <span data-ttu-id="8286f-157">用户上次查看或编辑文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-157">The date when user last viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages.</span></span> |
| <span data-ttu-id="8286f-158">skypeForBusinessLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8286f-158">skypeForBusinessLastActivityDate</span></span>  | <span data-ttu-id="8286f-159">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-159">Date</span></span>              | <span data-ttu-id="8286f-160">用户最后一次组织或参与会议的日期，或加入的对等会话。</span><span class="sxs-lookup"><span data-stu-id="8286f-160">The date when user last organized or participated in conferences, or joined peer-to-peer sessions.</span></span> |
| <span data-ttu-id="8286f-161">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8286f-161">yammerLastActivityDate</span></span>            | <span data-ttu-id="8286f-162">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-162">Date</span></span>              | <span data-ttu-id="8286f-163">用户上次发布、阅读或赞邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-163">The date when user last posted, read, or liked message.</span></span> |
| <span data-ttu-id="8286f-164">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8286f-164">teamsLastActivityDate</span></span>             | <span data-ttu-id="8286f-165">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-165">Date</span></span>              | <span data-ttu-id="8286f-166">用户上次在团队频道中发布的邮件，在私人聊天会话中发送的邮件，或参与会议或呼叫的日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-166">The date when user last posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls.</span></span> |
| <span data-ttu-id="8286f-167">exchangeLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8286f-167">exchangeLicenseAssignDate</span></span>         | <span data-ttu-id="8286f-168">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-168">Date</span></span>              | <span data-ttu-id="8286f-169">向用户分配 Exchange 许可证的最后日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-169">The last date when the user was assigned an Exchange license.</span></span> |
| <span data-ttu-id="8286f-170">oneDriveLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8286f-170">oneDriveLicenseAssignDate</span></span>         | <span data-ttu-id="8286f-171">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-171">Date</span></span>              | <span data-ttu-id="8286f-172">向用户分配 OneDrive 许可证的最后日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-172">The last date when the user was assigned a OneDrive license.</span></span> |
| <span data-ttu-id="8286f-173">sharePointLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8286f-173">sharePointLicenseAssignDate</span></span>       | <span data-ttu-id="8286f-174">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-174">Date</span></span>              | <span data-ttu-id="8286f-175">向用户分配 SharePoint 许可证的最后日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-175">The last date when the user was assigned a SharePoint license.</span></span> |
| <span data-ttu-id="8286f-176">skypeForBusinessLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8286f-176">skypeForBusinessLicenseAssignDate</span></span> | <span data-ttu-id="8286f-177">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-177">Date</span></span>              | <span data-ttu-id="8286f-178">为用户分配 Skype For Business 许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-178">The last date when the user was assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="8286f-179">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8286f-179">yammerLicenseAssignDate</span></span>           | <span data-ttu-id="8286f-180">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-180">Date</span></span>              | <span data-ttu-id="8286f-181">向用户分配 Yammer 许可证的最后日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-181">The last date when the user was assigned a Yammer license.</span></span> |
| <span data-ttu-id="8286f-182">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8286f-182">teamsLicenseAssignDate</span></span>            | <span data-ttu-id="8286f-183">日期</span><span class="sxs-lookup"><span data-stu-id="8286f-183">Date</span></span>              | <span data-ttu-id="8286f-184">向用户分配团队许可证的最后日期。</span><span class="sxs-lookup"><span data-stu-id="8286f-184">The last date when the user was assigned a Teams license.</span></span> |
| <span data-ttu-id="8286f-185">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="8286f-185">assignedProducts</span></span>                  | <span data-ttu-id="8286f-186">String 集合</span><span class="sxs-lookup"><span data-stu-id="8286f-186">String collection</span></span> | <span data-ttu-id="8286f-187">为用户分配的所有产品。</span><span class="sxs-lookup"><span data-stu-id="8286f-187">All the products assigned for the user.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8286f-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8286f-188">JSON representation</span></span>

<span data-ttu-id="8286f-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8286f-189">The following is a JSON representation of the resource.</span></span>

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
