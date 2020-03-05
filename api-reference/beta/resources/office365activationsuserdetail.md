---
title: office365ActivationsUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 45219f7666d4432bcdb2b409491338b94650a726
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522475"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="baa65-103">office365ActivationsUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="baa65-103">office365ActivationsUserDetail resource type</span></span>

<span data-ttu-id="baa65-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="baa65-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="baa65-105">属性</span><span class="sxs-lookup"><span data-stu-id="baa65-105">Properties</span></span>

| <span data-ttu-id="baa65-106">属性</span><span class="sxs-lookup"><span data-stu-id="baa65-106">Property</span></span>             | <span data-ttu-id="baa65-107">类型</span><span class="sxs-lookup"><span data-stu-id="baa65-107">Type</span></span>                                     | <span data-ttu-id="baa65-108">说明</span><span class="sxs-lookup"><span data-stu-id="baa65-108">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="baa65-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="baa65-109">reportRefreshDate</span></span>    | <span data-ttu-id="baa65-110">日期</span><span class="sxs-lookup"><span data-stu-id="baa65-110">Date</span></span>                                     | <span data-ttu-id="baa65-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="baa65-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="baa65-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="baa65-112">userPrincipalName</span></span>    | <span data-ttu-id="baa65-113">String</span><span class="sxs-lookup"><span data-stu-id="baa65-113">String</span></span>                                   | <span data-ttu-id="baa65-114">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="baa65-114">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="baa65-115">UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。</span><span class="sxs-lookup"><span data-stu-id="baa65-115">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="baa65-116">按照惯例，此名称应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="baa65-116">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="baa65-117">常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。</span><span class="sxs-lookup"><span data-stu-id="baa65-117">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="baa65-118">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="baa65-118">This property is required when a user is created.</span></span> |
| <span data-ttu-id="baa65-119">displayName</span><span class="sxs-lookup"><span data-stu-id="baa65-119">displayName</span></span>          | <span data-ttu-id="baa65-120">String</span><span class="sxs-lookup"><span data-stu-id="baa65-120">String</span></span>                                   | <span data-ttu-id="baa65-121">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="baa65-121">The name displayed in the address book for the user.</span></span> <span data-ttu-id="baa65-122">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="baa65-122">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="baa65-123">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="baa65-123">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="baa65-124">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="baa65-124">userActivationCounts</span></span> | <span data-ttu-id="baa65-125">[userActivationCounts](../resources/useractivationcounts.md)集合</span><span class="sxs-lookup"><span data-stu-id="baa65-125">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="baa65-126">用户的最新产品激活计数在所有分配的产品类型的所有平台上。</span><span class="sxs-lookup"><span data-stu-id="baa65-126">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="baa65-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="baa65-127">JSON representation</span></span>

<span data-ttu-id="baa65-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="baa65-128">The following is a JSON representation of the resource.</span></span>

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
