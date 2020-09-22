---
title: onPremisesProvisioningError 资源类型
description: 表示在将本地目录同步到 Azure Active Directory 时，用户、组或组织联系人实体的目录同步错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: japere
ms.openlocfilehash: ac6ae129374ab33e44a1f3274e8be378b90eb4e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052585"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="64e02-103">onPremisesProvisioningError 资源类型</span><span class="sxs-lookup"><span data-stu-id="64e02-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="64e02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64e02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64e02-105">表示在将本地目录同步到 Azure Active Directory 时， [用户](user.md)、 [组](group.md)或 [组织联系人](orgcontact.md) 实体的目录同步错误。</span><span class="sxs-lookup"><span data-stu-id="64e02-105">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="64e02-106">属性</span><span class="sxs-lookup"><span data-stu-id="64e02-106">Properties</span></span>

| <span data-ttu-id="64e02-107">属性</span><span class="sxs-lookup"><span data-stu-id="64e02-107">Property</span></span> | <span data-ttu-id="64e02-108">类型</span><span class="sxs-lookup"><span data-stu-id="64e02-108">Type</span></span> | <span data-ttu-id="64e02-109">说明</span><span class="sxs-lookup"><span data-stu-id="64e02-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="64e02-110">“类别”</span><span class="sxs-lookup"><span data-stu-id="64e02-110">category</span></span>|<span data-ttu-id="64e02-111">String</span><span class="sxs-lookup"><span data-stu-id="64e02-111">String</span></span>| <span data-ttu-id="64e02-112">设置错误的类别。</span><span class="sxs-lookup"><span data-stu-id="64e02-112">Category of the provisioning error.</span></span> <span data-ttu-id="64e02-113">注意：目前，只有一个可能的值。</span><span class="sxs-lookup"><span data-stu-id="64e02-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="64e02-114">可能的值： *PropertyConflict* -指示属性值不是唯一的。</span><span class="sxs-lookup"><span data-stu-id="64e02-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="64e02-115">其他对象包含相同的属性值。</span><span class="sxs-lookup"><span data-stu-id="64e02-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="64e02-116">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="64e02-116">occurredDateTime</span></span>|<span data-ttu-id="64e02-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64e02-117">DateTimeOffset</span></span>| <span data-ttu-id="64e02-118">发生错误的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="64e02-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="64e02-119">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="64e02-119">propertyCausingError</span></span>|<span data-ttu-id="64e02-120">String</span><span class="sxs-lookup"><span data-stu-id="64e02-120">String</span></span>| <span data-ttu-id="64e02-121">导致错误的目录属性的名称。</span><span class="sxs-lookup"><span data-stu-id="64e02-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="64e02-122">当前可能的值： *UserPrincipalName* 或 *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="64e02-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="64e02-123">value</span><span class="sxs-lookup"><span data-stu-id="64e02-123">value</span></span>|<span data-ttu-id="64e02-124">String</span><span class="sxs-lookup"><span data-stu-id="64e02-124">String</span></span>| <span data-ttu-id="64e02-125">导致错误的属性的值。</span><span class="sxs-lookup"><span data-stu-id="64e02-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64e02-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64e02-126">JSON representation</span></span>
<span data-ttu-id="64e02-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64e02-127">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


