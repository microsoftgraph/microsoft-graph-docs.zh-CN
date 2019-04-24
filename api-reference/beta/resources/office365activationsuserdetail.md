---
title: office365ActivationsUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a3561768e36fc63c779e19a9aa05863dd9af9315
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505492"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="df130-103">office365ActivationsUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="df130-103">office365ActivationsUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="df130-104">属性</span><span class="sxs-lookup"><span data-stu-id="df130-104">Properties</span></span>

| <span data-ttu-id="df130-105">属性</span><span class="sxs-lookup"><span data-stu-id="df130-105">Property</span></span>             | <span data-ttu-id="df130-106">类型</span><span class="sxs-lookup"><span data-stu-id="df130-106">Type</span></span>                                     | <span data-ttu-id="df130-107">说明</span><span class="sxs-lookup"><span data-stu-id="df130-107">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="df130-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="df130-108">reportRefreshDate</span></span>    | <span data-ttu-id="df130-109">Date</span><span class="sxs-lookup"><span data-stu-id="df130-109">Date</span></span>                                     | <span data-ttu-id="df130-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="df130-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="df130-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="df130-111">userPrincipalName</span></span>    | <span data-ttu-id="df130-112">String</span><span class="sxs-lookup"><span data-stu-id="df130-112">String</span></span>                                   | <span data-ttu-id="df130-113">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="df130-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="df130-114">UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。</span><span class="sxs-lookup"><span data-stu-id="df130-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="df130-115">按照惯例，此名称应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="df130-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="df130-116">常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。</span><span class="sxs-lookup"><span data-stu-id="df130-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="df130-117">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="df130-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="df130-118">displayName</span><span class="sxs-lookup"><span data-stu-id="df130-118">displayName</span></span>          | <span data-ttu-id="df130-119">String</span><span class="sxs-lookup"><span data-stu-id="df130-119">String</span></span>                                   | <span data-ttu-id="df130-120">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="df130-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="df130-121">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="df130-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="df130-122">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="df130-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="df130-123">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="df130-123">userActivationCounts</span></span> | <span data-ttu-id="df130-124">[userActivationCounts](../resources/useractivationcounts.md)集合</span><span class="sxs-lookup"><span data-stu-id="df130-124">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="df130-125">用户的最新产品激活计数在所有分配的产品类型的所有平台上。</span><span class="sxs-lookup"><span data-stu-id="df130-125">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="df130-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df130-126">JSON representation</span></span>

<span data-ttu-id="df130-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df130-127">The following is a JSON representation of the resource.</span></span>

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
