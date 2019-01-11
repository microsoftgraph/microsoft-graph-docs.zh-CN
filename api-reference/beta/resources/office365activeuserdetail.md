---
title: office365ActiveUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 462858f42b48560db4cd2f311ffdffd911504afe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833955"
---
# <a name="office365activeuserdetail-resource-type"></a><span data-ttu-id="8ff21-103">office365ActiveUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ff21-103">office365ActiveUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8ff21-104">属性</span><span class="sxs-lookup"><span data-stu-id="8ff21-104">Properties</span></span>

| <span data-ttu-id="8ff21-105">属性</span><span class="sxs-lookup"><span data-stu-id="8ff21-105">Property</span></span>                          | <span data-ttu-id="8ff21-106">类型</span><span class="sxs-lookup"><span data-stu-id="8ff21-106">Type</span></span>              | <span data-ttu-id="8ff21-107">Description</span><span class="sxs-lookup"><span data-stu-id="8ff21-107">Description</span></span>                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| <span data-ttu-id="8ff21-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-108">reportRefreshDate</span></span>                 | <span data-ttu-id="8ff21-109">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-109">Date</span></span>              | <span data-ttu-id="8ff21-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="8ff21-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="8ff21-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8ff21-111">userPrincipalName</span></span>                 | <span data-ttu-id="8ff21-112">字符串</span><span class="sxs-lookup"><span data-stu-id="8ff21-112">String</span></span>            | <span data-ttu-id="8ff21-113">用户主体名称 (UPN) 的用户。</span><span class="sxs-lookup"><span data-stu-id="8ff21-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="8ff21-114">UPN 是基于 Internet 标准 RFC 822 用户 Internet 风格登录名。</span><span class="sxs-lookup"><span data-stu-id="8ff21-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="8ff21-115">按照惯例，这应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="8ff21-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="8ff21-116">常规格式为 alias@domain，域必须存在于中的已验证域的租户的集合。</span><span class="sxs-lookup"><span data-stu-id="8ff21-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="8ff21-117">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="8ff21-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="8ff21-118">displayName</span><span class="sxs-lookup"><span data-stu-id="8ff21-118">displayName</span></span>                       | <span data-ttu-id="8ff21-119">String</span><span class="sxs-lookup"><span data-stu-id="8ff21-119">String</span></span>            | <span data-ttu-id="8ff21-120">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="8ff21-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="8ff21-121">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="8ff21-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="8ff21-122">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="8ff21-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="8ff21-123">被</span><span class="sxs-lookup"><span data-stu-id="8ff21-123">isDeleted</span></span>                         | <span data-ttu-id="8ff21-124">布尔</span><span class="sxs-lookup"><span data-stu-id="8ff21-124">Boolean</span></span>           | <span data-ttu-id="8ff21-125">此用户是否已被删除或软删除。</span><span class="sxs-lookup"><span data-stu-id="8ff21-125">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="8ff21-126">deletedDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-126">deletedDate</span></span>                       | <span data-ttu-id="8ff21-127">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-127">Date</span></span>              | <span data-ttu-id="8ff21-128">删除操作发生的日期。</span><span class="sxs-lookup"><span data-stu-id="8ff21-128">The date when the delete operation happened.</span></span> <span data-ttu-id="8ff21-129">用户未被删除时，默认值为"null"。</span><span class="sxs-lookup"><span data-stu-id="8ff21-129">Default value is "null" when the user has not been deleted.</span></span> |
| <span data-ttu-id="8ff21-130">hasExchangeLicense</span><span class="sxs-lookup"><span data-stu-id="8ff21-130">hasExchangeLicense</span></span>                | <span data-ttu-id="8ff21-131">布尔</span><span class="sxs-lookup"><span data-stu-id="8ff21-131">Boolean</span></span>           | <span data-ttu-id="8ff21-132">是否已分配用户的 Exchange 许可证。</span><span class="sxs-lookup"><span data-stu-id="8ff21-132">Whether the user has been assigned an Exchange license.</span></span> |
| <span data-ttu-id="8ff21-133">hasOneDriveLicense</span><span class="sxs-lookup"><span data-stu-id="8ff21-133">hasOneDriveLicense</span></span>                | <span data-ttu-id="8ff21-134">布尔</span><span class="sxs-lookup"><span data-stu-id="8ff21-134">Boolean</span></span>           | <span data-ttu-id="8ff21-135">是否具有已为用户分配 OneDrive 许可证。</span><span class="sxs-lookup"><span data-stu-id="8ff21-135">Whether the user has been assigned a OneDrive license.</span></span> |
| <span data-ttu-id="8ff21-136">hasSharePointLicense</span><span class="sxs-lookup"><span data-stu-id="8ff21-136">hasSharePointLicense</span></span>              | <span data-ttu-id="8ff21-137">布尔</span><span class="sxs-lookup"><span data-stu-id="8ff21-137">Boolean</span></span>           | <span data-ttu-id="8ff21-138">是否具有已为用户分配 SharePoint 许可证。</span><span class="sxs-lookup"><span data-stu-id="8ff21-138">Whether the user has been assigned a SharePoint license.</span></span> |
| <span data-ttu-id="8ff21-139">hasSkypeForBusinessLicense</span><span class="sxs-lookup"><span data-stu-id="8ff21-139">hasSkypeForBusinessLicense</span></span>        | <span data-ttu-id="8ff21-140">布尔</span><span class="sxs-lookup"><span data-stu-id="8ff21-140">Boolean</span></span>           | <span data-ttu-id="8ff21-141">是否具有已为用户分配 Skype 的业务许可证。</span><span class="sxs-lookup"><span data-stu-id="8ff21-141">Whether the user has been assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="8ff21-142">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="8ff21-142">hasYammerLicense</span></span>                  | <span data-ttu-id="8ff21-143">布尔</span><span class="sxs-lookup"><span data-stu-id="8ff21-143">Boolean</span></span>           | <span data-ttu-id="8ff21-144">是否具有已为用户分配 Yammer 许可证。</span><span class="sxs-lookup"><span data-stu-id="8ff21-144">Whether the user has been assigned a Yammer license.</span></span> |
| <span data-ttu-id="8ff21-145">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="8ff21-145">hasTeamsLicense</span></span>                   | <span data-ttu-id="8ff21-146">布尔</span><span class="sxs-lookup"><span data-stu-id="8ff21-146">Boolean</span></span>           | <span data-ttu-id="8ff21-147">是否具有已为用户分配的工作组许可证。</span><span class="sxs-lookup"><span data-stu-id="8ff21-147">Whether the user has been assigned a Teams license.</span></span> |
| <span data-ttu-id="8ff21-148">exchangeLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-148">exchangeLastActivityDate</span></span>          | <span data-ttu-id="8ff21-149">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-149">Date</span></span>              | <span data-ttu-id="8ff21-150">用户上次读取或发送电子邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="8ff21-150">The date when user last read or sent email.</span></span> |
| <span data-ttu-id="8ff21-151">oneDriveLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-151">oneDriveLastActivityDate</span></span>          | <span data-ttu-id="8ff21-152">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-152">Date</span></span>              | <span data-ttu-id="8ff21-153">用户上次查看或编辑文件的日期内部或外部，共享文件，或同步文件。</span><span class="sxs-lookup"><span data-stu-id="8ff21-153">The date when user last viewed or edited files, shared files internally or externally, or synced files.</span></span> |
| <span data-ttu-id="8ff21-154">sharePointLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-154">sharePointLastActivityDate</span></span>        | <span data-ttu-id="8ff21-155">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-155">Date</span></span>              | <span data-ttu-id="8ff21-156">用户上次查看或编辑文件的日期共享文件内部或外部同步文件，或查看 SharePoint 页面。</span><span class="sxs-lookup"><span data-stu-id="8ff21-156">The date when user last viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages.</span></span> |
| <span data-ttu-id="8ff21-157">skypeForBusinessLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-157">skypeForBusinessLastActivityDate</span></span>  | <span data-ttu-id="8ff21-158">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-158">Date</span></span>              | <span data-ttu-id="8ff21-159">当用户上次组织或参加会议，或加入对等会话的日期。</span><span class="sxs-lookup"><span data-stu-id="8ff21-159">The date when user last organized or participated in conferences, or joined peer-to-peer sessions.</span></span> |
| <span data-ttu-id="8ff21-160">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-160">yammerLastActivityDate</span></span>            | <span data-ttu-id="8ff21-161">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-161">Date</span></span>              | <span data-ttu-id="8ff21-162">当用户上次发布、 读取或喜欢消息日期。</span><span class="sxs-lookup"><span data-stu-id="8ff21-162">The date when user last posted, read, or liked message.</span></span> |
| <span data-ttu-id="8ff21-163">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-163">teamsLastActivityDate</span></span>             | <span data-ttu-id="8ff21-164">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-164">Date</span></span>              | <span data-ttu-id="8ff21-165">当用户上次发布消息团队通道中的日期私人聊天会话中发送的邮件，或参与会议或进行呼叫。</span><span class="sxs-lookup"><span data-stu-id="8ff21-165">The date when user last posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls.</span></span> |
| <span data-ttu-id="8ff21-166">exchangeLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-166">exchangeLicenseAssignDate</span></span>         | <span data-ttu-id="8ff21-167">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-167">Date</span></span>              | <span data-ttu-id="8ff21-168">用户已分配的 Exchange 许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="8ff21-168">The last date when the user was assigned an Exchange license.</span></span> |
| <span data-ttu-id="8ff21-169">oneDriveLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-169">oneDriveLicenseAssignDate</span></span>         | <span data-ttu-id="8ff21-170">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-170">Date</span></span>              | <span data-ttu-id="8ff21-171">用户已分配 OneDrive 许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="8ff21-171">The last date when the user was assigned a OneDrive license.</span></span> |
| <span data-ttu-id="8ff21-172">sharePointLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-172">sharePointLicenseAssignDate</span></span>       | <span data-ttu-id="8ff21-173">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-173">Date</span></span>              | <span data-ttu-id="8ff21-174">用户已分配 SharePoint 许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="8ff21-174">The last date when the user was assigned a SharePoint license.</span></span> |
| <span data-ttu-id="8ff21-175">skypeForBusinessLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-175">skypeForBusinessLicenseAssignDate</span></span> | <span data-ttu-id="8ff21-176">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-176">Date</span></span>              | <span data-ttu-id="8ff21-177">用户已分配的 Skype 的业务许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="8ff21-177">The last date when the user was assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="8ff21-178">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-178">yammerLicenseAssignDate</span></span>           | <span data-ttu-id="8ff21-179">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-179">Date</span></span>              | <span data-ttu-id="8ff21-180">用户已分配的 Yammer 许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="8ff21-180">The last date when the user was assigned a Yammer license.</span></span> |
| <span data-ttu-id="8ff21-181">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="8ff21-181">teamsLicenseAssignDate</span></span>            | <span data-ttu-id="8ff21-182">日期</span><span class="sxs-lookup"><span data-stu-id="8ff21-182">Date</span></span>              | <span data-ttu-id="8ff21-183">用户已分配的团队许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="8ff21-183">The last date when the user was assigned a Teams license.</span></span> |
| <span data-ttu-id="8ff21-184">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="8ff21-184">assignedProducts</span></span>                  | <span data-ttu-id="8ff21-185">String 集合</span><span class="sxs-lookup"><span data-stu-id="8ff21-185">String collection</span></span> | <span data-ttu-id="8ff21-186">为用户分配的所有产品。</span><span class="sxs-lookup"><span data-stu-id="8ff21-186">All the products assigned for the user.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8ff21-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ff21-187">JSON representation</span></span>

<span data-ttu-id="8ff21-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ff21-188">The following is a JSON representation of the resource.</span></span>

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
