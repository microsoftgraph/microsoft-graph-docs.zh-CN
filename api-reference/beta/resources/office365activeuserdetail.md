---
title: office365ActiveUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 14c785069868783b1e248b41a5b339c9adb4710a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929281"
---
# <a name="office365activeuserdetail-resource-type"></a><span data-ttu-id="d2c65-103">office365ActiveUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2c65-103">office365ActiveUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d2c65-104">属性</span><span class="sxs-lookup"><span data-stu-id="d2c65-104">Properties</span></span>

| <span data-ttu-id="d2c65-105">属性</span><span class="sxs-lookup"><span data-stu-id="d2c65-105">Property</span></span>                          | <span data-ttu-id="d2c65-106">类型</span><span class="sxs-lookup"><span data-stu-id="d2c65-106">Type</span></span>              | <span data-ttu-id="d2c65-107">说明</span><span class="sxs-lookup"><span data-stu-id="d2c65-107">Description</span></span>                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| <span data-ttu-id="d2c65-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-108">reportRefreshDate</span></span>                 | <span data-ttu-id="d2c65-109">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-109">Date</span></span>              | <span data-ttu-id="d2c65-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="d2c65-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="d2c65-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d2c65-111">userPrincipalName</span></span>                 | <span data-ttu-id="d2c65-112">字符串</span><span class="sxs-lookup"><span data-stu-id="d2c65-112">String</span></span>            | <span data-ttu-id="d2c65-113">用户主体名称 (UPN) 的用户。</span><span class="sxs-lookup"><span data-stu-id="d2c65-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="d2c65-114">UPN 是基于 Internet 标准 RFC 822 用户 Internet 风格登录名。</span><span class="sxs-lookup"><span data-stu-id="d2c65-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="d2c65-115">按照惯例，这应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="d2c65-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="d2c65-116">常规格式为 alias@domain，域必须存在于中的已验证域的租户的集合。</span><span class="sxs-lookup"><span data-stu-id="d2c65-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="d2c65-117">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="d2c65-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="d2c65-118">displayName</span><span class="sxs-lookup"><span data-stu-id="d2c65-118">displayName</span></span>                       | <span data-ttu-id="d2c65-119">String</span><span class="sxs-lookup"><span data-stu-id="d2c65-119">String</span></span>            | <span data-ttu-id="d2c65-120">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="d2c65-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="d2c65-121">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="d2c65-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="d2c65-122">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="d2c65-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="d2c65-123">被</span><span class="sxs-lookup"><span data-stu-id="d2c65-123">isDeleted</span></span>                         | <span data-ttu-id="d2c65-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2c65-124">Boolean</span></span>           | <span data-ttu-id="d2c65-125">此用户是否已被删除或软删除。</span><span class="sxs-lookup"><span data-stu-id="d2c65-125">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="d2c65-126">deletedDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-126">deletedDate</span></span>                       | <span data-ttu-id="d2c65-127">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-127">Date</span></span>              | <span data-ttu-id="d2c65-128">删除操作发生的日期。</span><span class="sxs-lookup"><span data-stu-id="d2c65-128">The date when the delete operation happened.</span></span> <span data-ttu-id="d2c65-129">用户未被删除时，默认值为"null"。</span><span class="sxs-lookup"><span data-stu-id="d2c65-129">Default value is "null" when the user has not been deleted.</span></span> |
| <span data-ttu-id="d2c65-130">hasExchangeLicense</span><span class="sxs-lookup"><span data-stu-id="d2c65-130">hasExchangeLicense</span></span>                | <span data-ttu-id="d2c65-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2c65-131">Boolean</span></span>           | <span data-ttu-id="d2c65-132">是否已分配用户的 Exchange 许可证。</span><span class="sxs-lookup"><span data-stu-id="d2c65-132">Whether the user has been assigned an Exchange license.</span></span> |
| <span data-ttu-id="d2c65-133">hasOneDriveLicense</span><span class="sxs-lookup"><span data-stu-id="d2c65-133">hasOneDriveLicense</span></span>                | <span data-ttu-id="d2c65-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2c65-134">Boolean</span></span>           | <span data-ttu-id="d2c65-135">是否具有已为用户分配 OneDrive 许可证。</span><span class="sxs-lookup"><span data-stu-id="d2c65-135">Whether the user has been assigned a OneDrive license.</span></span> |
| <span data-ttu-id="d2c65-136">hasSharePointLicense</span><span class="sxs-lookup"><span data-stu-id="d2c65-136">hasSharePointLicense</span></span>              | <span data-ttu-id="d2c65-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2c65-137">Boolean</span></span>           | <span data-ttu-id="d2c65-138">是否具有已为用户分配 SharePoint 许可证。</span><span class="sxs-lookup"><span data-stu-id="d2c65-138">Whether the user has been assigned a SharePoint license.</span></span> |
| <span data-ttu-id="d2c65-139">hasSkypeForBusinessLicense</span><span class="sxs-lookup"><span data-stu-id="d2c65-139">hasSkypeForBusinessLicense</span></span>        | <span data-ttu-id="d2c65-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2c65-140">Boolean</span></span>           | <span data-ttu-id="d2c65-141">是否具有已为用户分配 Skype 的业务许可证。</span><span class="sxs-lookup"><span data-stu-id="d2c65-141">Whether the user has been assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="d2c65-142">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="d2c65-142">hasYammerLicense</span></span>                  | <span data-ttu-id="d2c65-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2c65-143">Boolean</span></span>           | <span data-ttu-id="d2c65-144">是否具有已为用户分配 Yammer 许可证。</span><span class="sxs-lookup"><span data-stu-id="d2c65-144">Whether the user has been assigned a Yammer license.</span></span> |
| <span data-ttu-id="d2c65-145">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="d2c65-145">hasTeamsLicense</span></span>                   | <span data-ttu-id="d2c65-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2c65-146">Boolean</span></span>           | <span data-ttu-id="d2c65-147">是否具有已为用户分配的工作组许可证。</span><span class="sxs-lookup"><span data-stu-id="d2c65-147">Whether the user has been assigned a Teams license.</span></span> |
| <span data-ttu-id="d2c65-148">exchangeLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-148">exchangeLastActivityDate</span></span>          | <span data-ttu-id="d2c65-149">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-149">Date</span></span>              | <span data-ttu-id="d2c65-150">用户上次读取或发送电子邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="d2c65-150">The date when user last read or sent email.</span></span> |
| <span data-ttu-id="d2c65-151">oneDriveLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-151">oneDriveLastActivityDate</span></span>          | <span data-ttu-id="d2c65-152">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-152">Date</span></span>              | <span data-ttu-id="d2c65-153">用户上次查看或编辑文件的日期内部或外部，共享文件，或同步文件。</span><span class="sxs-lookup"><span data-stu-id="d2c65-153">The date when user last viewed or edited files, shared files internally or externally, or synced files.</span></span> |
| <span data-ttu-id="d2c65-154">sharePointLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-154">sharePointLastActivityDate</span></span>        | <span data-ttu-id="d2c65-155">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-155">Date</span></span>              | <span data-ttu-id="d2c65-156">用户上次查看或编辑文件的日期共享文件内部或外部同步文件，或查看 SharePoint 页面。</span><span class="sxs-lookup"><span data-stu-id="d2c65-156">The date when user last viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages.</span></span> |
| <span data-ttu-id="d2c65-157">skypeForBusinessLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-157">skypeForBusinessLastActivityDate</span></span>  | <span data-ttu-id="d2c65-158">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-158">Date</span></span>              | <span data-ttu-id="d2c65-159">当用户上次组织或参加会议，或加入对等会话的日期。</span><span class="sxs-lookup"><span data-stu-id="d2c65-159">The date when user last organized or participated in conferences, or joined peer-to-peer sessions.</span></span> |
| <span data-ttu-id="d2c65-160">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-160">yammerLastActivityDate</span></span>            | <span data-ttu-id="d2c65-161">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-161">Date</span></span>              | <span data-ttu-id="d2c65-162">当用户上次发布、 读取或喜欢消息日期。</span><span class="sxs-lookup"><span data-stu-id="d2c65-162">The date when user last posted, read, or liked message.</span></span> |
| <span data-ttu-id="d2c65-163">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-163">teamsLastActivityDate</span></span>             | <span data-ttu-id="d2c65-164">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-164">Date</span></span>              | <span data-ttu-id="d2c65-165">当用户上次发布消息团队通道中的日期私人聊天会话中发送的邮件，或参与会议或进行呼叫。</span><span class="sxs-lookup"><span data-stu-id="d2c65-165">The date when user last posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls.</span></span> |
| <span data-ttu-id="d2c65-166">exchangeLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-166">exchangeLicenseAssignDate</span></span>         | <span data-ttu-id="d2c65-167">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-167">Date</span></span>              | <span data-ttu-id="d2c65-168">用户已分配的 Exchange 许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="d2c65-168">The last date when the user was assigned an Exchange license.</span></span> |
| <span data-ttu-id="d2c65-169">oneDriveLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-169">oneDriveLicenseAssignDate</span></span>         | <span data-ttu-id="d2c65-170">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-170">Date</span></span>              | <span data-ttu-id="d2c65-171">用户已分配 OneDrive 许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="d2c65-171">The last date when the user was assigned a OneDrive license.</span></span> |
| <span data-ttu-id="d2c65-172">sharePointLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-172">sharePointLicenseAssignDate</span></span>       | <span data-ttu-id="d2c65-173">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-173">Date</span></span>              | <span data-ttu-id="d2c65-174">用户已分配 SharePoint 许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="d2c65-174">The last date when the user was assigned a SharePoint license.</span></span> |
| <span data-ttu-id="d2c65-175">skypeForBusinessLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-175">skypeForBusinessLicenseAssignDate</span></span> | <span data-ttu-id="d2c65-176">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-176">Date</span></span>              | <span data-ttu-id="d2c65-177">用户已分配的 Skype 的业务许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="d2c65-177">The last date when the user was assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="d2c65-178">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-178">yammerLicenseAssignDate</span></span>           | <span data-ttu-id="d2c65-179">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-179">Date</span></span>              | <span data-ttu-id="d2c65-180">用户已分配的 Yammer 许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="d2c65-180">The last date when the user was assigned a Yammer license.</span></span> |
| <span data-ttu-id="d2c65-181">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="d2c65-181">teamsLicenseAssignDate</span></span>            | <span data-ttu-id="d2c65-182">日期</span><span class="sxs-lookup"><span data-stu-id="d2c65-182">Date</span></span>              | <span data-ttu-id="d2c65-183">用户已分配的团队许可证的最后一个日期。</span><span class="sxs-lookup"><span data-stu-id="d2c65-183">The last date when the user was assigned a Teams license.</span></span> |
| <span data-ttu-id="d2c65-184">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="d2c65-184">assignedProducts</span></span>                  | <span data-ttu-id="d2c65-185">String 集合</span><span class="sxs-lookup"><span data-stu-id="d2c65-185">String collection</span></span> | <span data-ttu-id="d2c65-186">为用户分配的所有产品。</span><span class="sxs-lookup"><span data-stu-id="d2c65-186">All the products assigned for the user.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d2c65-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2c65-187">JSON representation</span></span>

<span data-ttu-id="d2c65-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2c65-188">The following is a JSON representation of the resource.</span></span>

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
