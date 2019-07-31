---
title: office365ActiveUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 9e58e0d4613118cd8ceecfcae318982bc2035917
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009494"
---
# <a name="office365activeuserdetail-resource-type"></a><span data-ttu-id="041bd-103">office365ActiveUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="041bd-103">office365ActiveUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="041bd-104">属性</span><span class="sxs-lookup"><span data-stu-id="041bd-104">Properties</span></span>

| <span data-ttu-id="041bd-105">属性</span><span class="sxs-lookup"><span data-stu-id="041bd-105">Property</span></span>                          | <span data-ttu-id="041bd-106">类型</span><span class="sxs-lookup"><span data-stu-id="041bd-106">Type</span></span>              | <span data-ttu-id="041bd-107">说明</span><span class="sxs-lookup"><span data-stu-id="041bd-107">Description</span></span>                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| <span data-ttu-id="041bd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="041bd-108">reportRefreshDate</span></span>                 | <span data-ttu-id="041bd-109">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-109">Date</span></span>              | <span data-ttu-id="041bd-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="041bd-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="041bd-111">userPrincipalName</span></span>                 | <span data-ttu-id="041bd-112">String</span><span class="sxs-lookup"><span data-stu-id="041bd-112">String</span></span>            | <span data-ttu-id="041bd-113">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="041bd-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="041bd-114">UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。</span><span class="sxs-lookup"><span data-stu-id="041bd-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="041bd-115">按照惯例，此名称应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="041bd-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="041bd-116">常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。</span><span class="sxs-lookup"><span data-stu-id="041bd-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="041bd-117">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="041bd-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="041bd-118">displayName</span><span class="sxs-lookup"><span data-stu-id="041bd-118">displayName</span></span>                       | <span data-ttu-id="041bd-119">String</span><span class="sxs-lookup"><span data-stu-id="041bd-119">String</span></span>            | <span data-ttu-id="041bd-120">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="041bd-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="041bd-121">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="041bd-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="041bd-122">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="041bd-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="041bd-123">isDeleted</span><span class="sxs-lookup"><span data-stu-id="041bd-123">isDeleted</span></span>                         | <span data-ttu-id="041bd-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="041bd-124">Boolean</span></span>           | <span data-ttu-id="041bd-125">此用户是否已被删除或软删除。</span><span class="sxs-lookup"><span data-stu-id="041bd-125">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="041bd-126">deletedDate</span><span class="sxs-lookup"><span data-stu-id="041bd-126">deletedDate</span></span>                       | <span data-ttu-id="041bd-127">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-127">Date</span></span>              | <span data-ttu-id="041bd-128">删除操作发生的日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-128">The date when the delete operation happened.</span></span> <span data-ttu-id="041bd-129">当用户未被删除时, 默认值为 "null"。</span><span class="sxs-lookup"><span data-stu-id="041bd-129">Default value is "null" when the user has not been deleted.</span></span> |
| <span data-ttu-id="041bd-130">hasExchangeLicense</span><span class="sxs-lookup"><span data-stu-id="041bd-130">hasExchangeLicense</span></span>                | <span data-ttu-id="041bd-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="041bd-131">Boolean</span></span>           | <span data-ttu-id="041bd-132">是否已为用户分配了 Exchange 许可证。</span><span class="sxs-lookup"><span data-stu-id="041bd-132">Whether the user has been assigned an Exchange license.</span></span> |
| <span data-ttu-id="041bd-133">hasOneDriveLicense</span><span class="sxs-lookup"><span data-stu-id="041bd-133">hasOneDriveLicense</span></span>                | <span data-ttu-id="041bd-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="041bd-134">Boolean</span></span>           | <span data-ttu-id="041bd-135">是否已为用户分配 OneDrive 许可证。</span><span class="sxs-lookup"><span data-stu-id="041bd-135">Whether the user has been assigned a OneDrive license.</span></span> |
| <span data-ttu-id="041bd-136">hasSharePointLicense</span><span class="sxs-lookup"><span data-stu-id="041bd-136">hasSharePointLicense</span></span>              | <span data-ttu-id="041bd-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="041bd-137">Boolean</span></span>           | <span data-ttu-id="041bd-138">是否已为用户分配 SharePoint 许可证。</span><span class="sxs-lookup"><span data-stu-id="041bd-138">Whether the user has been assigned a SharePoint license.</span></span> |
| <span data-ttu-id="041bd-139">hasSkypeForBusinessLicense</span><span class="sxs-lookup"><span data-stu-id="041bd-139">hasSkypeForBusinessLicense</span></span>        | <span data-ttu-id="041bd-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="041bd-140">Boolean</span></span>           | <span data-ttu-id="041bd-141">是否已为用户分配 Skype For Business 许可证。</span><span class="sxs-lookup"><span data-stu-id="041bd-141">Whether the user has been assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="041bd-142">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="041bd-142">hasYammerLicense</span></span>                  | <span data-ttu-id="041bd-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="041bd-143">Boolean</span></span>           | <span data-ttu-id="041bd-144">是否为用户分配了 Yammer 许可证。</span><span class="sxs-lookup"><span data-stu-id="041bd-144">Whether the user has been assigned a Yammer license.</span></span> |
| <span data-ttu-id="041bd-145">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="041bd-145">hasTeamsLicense</span></span>                   | <span data-ttu-id="041bd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="041bd-146">Boolean</span></span>           | <span data-ttu-id="041bd-147">是否已向用户分配团队许可证。</span><span class="sxs-lookup"><span data-stu-id="041bd-147">Whether the user has been assigned a Teams license.</span></span> |
| <span data-ttu-id="041bd-148">exchangeLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="041bd-148">exchangeLastActivityDate</span></span>          | <span data-ttu-id="041bd-149">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-149">Date</span></span>              | <span data-ttu-id="041bd-150">用户最后一次阅读或发送电子邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-150">The date when user last read or sent email.</span></span> |
| <span data-ttu-id="041bd-151">oneDriveLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="041bd-151">oneDriveLastActivityDate</span></span>          | <span data-ttu-id="041bd-152">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-152">Date</span></span>              | <span data-ttu-id="041bd-153">用户上次查看或编辑文件、内部或外部共享文件或同步文件的日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-153">The date when user last viewed or edited files, shared files internally or externally, or synced files.</span></span> |
| <span data-ttu-id="041bd-154">sharePointLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="041bd-154">sharePointLastActivityDate</span></span>        | <span data-ttu-id="041bd-155">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-155">Date</span></span>              | <span data-ttu-id="041bd-156">用户上次查看或编辑文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-156">The date when user last viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages.</span></span> |
| <span data-ttu-id="041bd-157">skypeForBusinessLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="041bd-157">skypeForBusinessLastActivityDate</span></span>  | <span data-ttu-id="041bd-158">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-158">Date</span></span>              | <span data-ttu-id="041bd-159">用户最后一次组织或参与会议的日期, 或加入的对等会话。</span><span class="sxs-lookup"><span data-stu-id="041bd-159">The date when user last organized or participated in conferences, or joined peer-to-peer sessions.</span></span> |
| <span data-ttu-id="041bd-160">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="041bd-160">yammerLastActivityDate</span></span>            | <span data-ttu-id="041bd-161">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-161">Date</span></span>              | <span data-ttu-id="041bd-162">用户上次发布、阅读或赞邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-162">The date when user last posted, read, or liked message.</span></span> |
| <span data-ttu-id="041bd-163">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="041bd-163">teamsLastActivityDate</span></span>             | <span data-ttu-id="041bd-164">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-164">Date</span></span>              | <span data-ttu-id="041bd-165">用户上次在团队频道中发布的邮件, 在私人聊天会话中发送的邮件, 或参与会议或呼叫的日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-165">The date when user last posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls.</span></span> |
| <span data-ttu-id="041bd-166">exchangeLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="041bd-166">exchangeLicenseAssignDate</span></span>         | <span data-ttu-id="041bd-167">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-167">Date</span></span>              | <span data-ttu-id="041bd-168">向用户分配 Exchange 许可证的最后日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-168">The last date when the user was assigned an Exchange license.</span></span> |
| <span data-ttu-id="041bd-169">oneDriveLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="041bd-169">oneDriveLicenseAssignDate</span></span>         | <span data-ttu-id="041bd-170">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-170">Date</span></span>              | <span data-ttu-id="041bd-171">向用户分配 OneDrive 许可证的最后日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-171">The last date when the user was assigned a OneDrive license.</span></span> |
| <span data-ttu-id="041bd-172">sharePointLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="041bd-172">sharePointLicenseAssignDate</span></span>       | <span data-ttu-id="041bd-173">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-173">Date</span></span>              | <span data-ttu-id="041bd-174">向用户分配 SharePoint 许可证的最后日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-174">The last date when the user was assigned a SharePoint license.</span></span> |
| <span data-ttu-id="041bd-175">skypeForBusinessLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="041bd-175">skypeForBusinessLicenseAssignDate</span></span> | <span data-ttu-id="041bd-176">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-176">Date</span></span>              | <span data-ttu-id="041bd-177">为用户分配 Skype For Business 许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-177">The last date when the user was assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="041bd-178">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="041bd-178">yammerLicenseAssignDate</span></span>           | <span data-ttu-id="041bd-179">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-179">Date</span></span>              | <span data-ttu-id="041bd-180">向用户分配 Yammer 许可证的最后日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-180">The last date when the user was assigned a Yammer license.</span></span> |
| <span data-ttu-id="041bd-181">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="041bd-181">teamsLicenseAssignDate</span></span>            | <span data-ttu-id="041bd-182">日期</span><span class="sxs-lookup"><span data-stu-id="041bd-182">Date</span></span>              | <span data-ttu-id="041bd-183">向用户分配团队许可证的最后日期。</span><span class="sxs-lookup"><span data-stu-id="041bd-183">The last date when the user was assigned a Teams license.</span></span> |
| <span data-ttu-id="041bd-184">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="041bd-184">assignedProducts</span></span>                  | <span data-ttu-id="041bd-185">String collection</span><span class="sxs-lookup"><span data-stu-id="041bd-185">String collection</span></span> | <span data-ttu-id="041bd-186">为用户分配的所有产品。</span><span class="sxs-lookup"><span data-stu-id="041bd-186">All the products assigned for the user.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="041bd-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="041bd-187">JSON representation</span></span>

<span data-ttu-id="041bd-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="041bd-188">The following is a JSON representation of the resource.</span></span>

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
