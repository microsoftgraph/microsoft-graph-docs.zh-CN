---
title: onPremisesProvisioningError 资源类型
description: 表示将本地目录同步到 Azure Active Directory 时用户组和联系人资源的目录同步错误。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 719bb525fad934bb92f44fb427d1214bf288ec46
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059087"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="017bd-103">onPremisesProvisioningError 资源类型</span><span class="sxs-lookup"><span data-stu-id="017bd-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="017bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="017bd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="017bd-105">表示将本地目录同步到 Azure Active Directory 时 [用户](user.md)、 [组](group.md) 和 [orgContact](orgcontact.md) 资源的目录同步错误。</span><span class="sxs-lookup"><span data-stu-id="017bd-105">Represents directory synchronization errors for the [user](user.md), [group](group.md) and [orgContact](orgcontact.md) resources when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="017bd-106">属性</span><span class="sxs-lookup"><span data-stu-id="017bd-106">Properties</span></span>

| <span data-ttu-id="017bd-107">属性</span><span class="sxs-lookup"><span data-stu-id="017bd-107">Property</span></span> | <span data-ttu-id="017bd-108">类型</span><span class="sxs-lookup"><span data-stu-id="017bd-108">Type</span></span> | <span data-ttu-id="017bd-109">说明</span><span class="sxs-lookup"><span data-stu-id="017bd-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="017bd-110">“类别”</span><span class="sxs-lookup"><span data-stu-id="017bd-110">category</span></span>|<span data-ttu-id="017bd-111">String</span><span class="sxs-lookup"><span data-stu-id="017bd-111">String</span></span>| <span data-ttu-id="017bd-112">设置错误的类别。</span><span class="sxs-lookup"><span data-stu-id="017bd-112">Category of the provisioning error.</span></span> <span data-ttu-id="017bd-113">注意：目前，只有一个可能的值。</span><span class="sxs-lookup"><span data-stu-id="017bd-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="017bd-114">可能的值： *PropertyConflict* -指示属性值不是唯一的。</span><span class="sxs-lookup"><span data-stu-id="017bd-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="017bd-115">其他对象包含相同的属性值。</span><span class="sxs-lookup"><span data-stu-id="017bd-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="017bd-116">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="017bd-116">occurredDateTime</span></span>|<span data-ttu-id="017bd-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="017bd-117">DateTimeOffset</span></span>| <span data-ttu-id="017bd-118">发生错误的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="017bd-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="017bd-119">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="017bd-119">propertyCausingError</span></span>|<span data-ttu-id="017bd-120">String</span><span class="sxs-lookup"><span data-stu-id="017bd-120">String</span></span>| <span data-ttu-id="017bd-121">导致错误的目录属性的名称。</span><span class="sxs-lookup"><span data-stu-id="017bd-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="017bd-122">当前可能的值： *UserPrincipalName* 或 *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="017bd-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="017bd-123">value</span><span class="sxs-lookup"><span data-stu-id="017bd-123">value</span></span>|<span data-ttu-id="017bd-124">String</span><span class="sxs-lookup"><span data-stu-id="017bd-124">String</span></span>| <span data-ttu-id="017bd-125">导致错误的属性的值。</span><span class="sxs-lookup"><span data-stu-id="017bd-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="017bd-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="017bd-126">JSON representation</span></span>
<span data-ttu-id="017bd-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="017bd-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

