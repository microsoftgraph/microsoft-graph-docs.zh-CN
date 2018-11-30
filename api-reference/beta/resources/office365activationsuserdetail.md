---
title: office365ActivationsUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 9cf0f7f841584654176c0069fb0403a86615bfd5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043648"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="5a93b-103">office365ActivationsUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a93b-103">office365ActivationsUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5a93b-104">属性</span><span class="sxs-lookup"><span data-stu-id="5a93b-104">Properties</span></span>

| <span data-ttu-id="5a93b-105">属性</span><span class="sxs-lookup"><span data-stu-id="5a93b-105">Property</span></span>             | <span data-ttu-id="5a93b-106">类型</span><span class="sxs-lookup"><span data-stu-id="5a93b-106">Type</span></span>                                     | <span data-ttu-id="5a93b-107">说明</span><span class="sxs-lookup"><span data-stu-id="5a93b-107">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="5a93b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5a93b-108">reportRefreshDate</span></span>    | <span data-ttu-id="5a93b-109">日期</span><span class="sxs-lookup"><span data-stu-id="5a93b-109">Date</span></span>                                     | <span data-ttu-id="5a93b-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="5a93b-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="5a93b-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5a93b-111">userPrincipalName</span></span>    | <span data-ttu-id="5a93b-112">字符串</span><span class="sxs-lookup"><span data-stu-id="5a93b-112">String</span></span>                                   | <span data-ttu-id="5a93b-113">用户主体名称 (UPN) 的用户。</span><span class="sxs-lookup"><span data-stu-id="5a93b-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="5a93b-114">UPN 是基于 Internet 标准 RFC 822 用户 Internet 风格登录名。</span><span class="sxs-lookup"><span data-stu-id="5a93b-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="5a93b-115">按照惯例，这应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="5a93b-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="5a93b-116">常规格式为 alias@domain，域必须存在于中的已验证域的租户的集合。</span><span class="sxs-lookup"><span data-stu-id="5a93b-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="5a93b-117">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="5a93b-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="5a93b-118">displayName</span><span class="sxs-lookup"><span data-stu-id="5a93b-118">displayName</span></span>          | <span data-ttu-id="5a93b-119">String</span><span class="sxs-lookup"><span data-stu-id="5a93b-119">String</span></span>                                   | <span data-ttu-id="5a93b-120">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="5a93b-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="5a93b-121">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="5a93b-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="5a93b-122">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="5a93b-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="5a93b-123">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="5a93b-123">userActivationCounts</span></span> | <span data-ttu-id="5a93b-124">[userActivationCounts](../resources/useractivationcounts.md)集合</span><span class="sxs-lookup"><span data-stu-id="5a93b-124">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="5a93b-125">用户的最新的产品激活计算的所有已分配的产品类型的所有平台上。</span><span class="sxs-lookup"><span data-stu-id="5a93b-125">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a93b-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a93b-126">JSON representation</span></span>

<span data-ttu-id="5a93b-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a93b-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userActivationCounts": [{"@odata.type":"microsoft.graph.userActivationCounts"}]
}
```
