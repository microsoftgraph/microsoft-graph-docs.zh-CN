---
title: office365ActivationsUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3e2b7d5fb3c42db02407a187649544b2560f898a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982853"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="76088-103">office365ActivationsUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="76088-103">office365ActivationsUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="76088-104">属性</span><span class="sxs-lookup"><span data-stu-id="76088-104">Properties</span></span>

| <span data-ttu-id="76088-105">属性</span><span class="sxs-lookup"><span data-stu-id="76088-105">Property</span></span>             | <span data-ttu-id="76088-106">类型</span><span class="sxs-lookup"><span data-stu-id="76088-106">Type</span></span>                                     | <span data-ttu-id="76088-107">说明</span><span class="sxs-lookup"><span data-stu-id="76088-107">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="76088-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="76088-108">reportRefreshDate</span></span>    | <span data-ttu-id="76088-109">日期</span><span class="sxs-lookup"><span data-stu-id="76088-109">Date</span></span>                                     | <span data-ttu-id="76088-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="76088-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="76088-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="76088-111">userPrincipalName</span></span>    | <span data-ttu-id="76088-112">字符串</span><span class="sxs-lookup"><span data-stu-id="76088-112">String</span></span>                                   | <span data-ttu-id="76088-113">用户主体名称 (UPN) 的用户。</span><span class="sxs-lookup"><span data-stu-id="76088-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="76088-114">UPN 是基于 Internet 标准 RFC 822 用户 Internet 风格登录名。</span><span class="sxs-lookup"><span data-stu-id="76088-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="76088-115">按照惯例，这应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="76088-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="76088-116">常规格式为 alias@domain，域必须存在于中的已验证域的租户的集合。</span><span class="sxs-lookup"><span data-stu-id="76088-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="76088-117">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="76088-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="76088-118">displayName</span><span class="sxs-lookup"><span data-stu-id="76088-118">displayName</span></span>          | <span data-ttu-id="76088-119">String</span><span class="sxs-lookup"><span data-stu-id="76088-119">String</span></span>                                   | <span data-ttu-id="76088-120">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="76088-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="76088-121">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="76088-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="76088-122">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="76088-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="76088-123">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="76088-123">userActivationCounts</span></span> | <span data-ttu-id="76088-124">[userActivationCounts](../resources/useractivationcounts.md)集合</span><span class="sxs-lookup"><span data-stu-id="76088-124">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="76088-125">用户的最新的产品激活计算的所有已分配的产品类型的所有平台上。</span><span class="sxs-lookup"><span data-stu-id="76088-125">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76088-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76088-126">JSON representation</span></span>

<span data-ttu-id="76088-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76088-127">The following is a JSON representation of the resource.</span></span>

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
