---
title: onPremisesProvisioningError 资源类型
description: 表示将本地目录同步到 Azure Active Directory 时用户组和联系人资源的目录同步错误。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ccbb10bdf5dba14a01a572198dbdbbafb2534eb7
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621650"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="b4837-103">onPremisesProvisioningError 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4837-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="b4837-104">表示将本地目录同步到 Azure Active Directory 时[用户](user.md)、[组](group.md)和[orgContact](orgcontact.md)资源的目录同步错误。</span><span class="sxs-lookup"><span data-stu-id="b4837-104">Represents directory synchronization errors for the [user](user.md), [group](group.md) and [orgContact](orgcontact.md) resources when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="b4837-105">属性</span><span class="sxs-lookup"><span data-stu-id="b4837-105">Properties</span></span>

| <span data-ttu-id="b4837-106">属性</span><span class="sxs-lookup"><span data-stu-id="b4837-106">Property</span></span> | <span data-ttu-id="b4837-107">类型</span><span class="sxs-lookup"><span data-stu-id="b4837-107">Type</span></span> | <span data-ttu-id="b4837-108">说明</span><span class="sxs-lookup"><span data-stu-id="b4837-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b4837-109">“类别”</span><span class="sxs-lookup"><span data-stu-id="b4837-109">category</span></span>|<span data-ttu-id="b4837-110">String</span><span class="sxs-lookup"><span data-stu-id="b4837-110">String</span></span>| <span data-ttu-id="b4837-111">设置错误的类别。</span><span class="sxs-lookup"><span data-stu-id="b4837-111">Category of the provisioning error.</span></span> <span data-ttu-id="b4837-112">注意：目前，只有一个可能的值。</span><span class="sxs-lookup"><span data-stu-id="b4837-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="b4837-113">可能的值： *PropertyConflict* -指示属性值不是唯一的。</span><span class="sxs-lookup"><span data-stu-id="b4837-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="b4837-114">其他对象包含相同的属性值。</span><span class="sxs-lookup"><span data-stu-id="b4837-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="b4837-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="b4837-115">occurredDateTime</span></span>|<span data-ttu-id="b4837-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4837-116">DateTimeOffset</span></span>| <span data-ttu-id="b4837-117">发生错误的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b4837-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="b4837-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="b4837-118">propertyCausingError</span></span>|<span data-ttu-id="b4837-119">String</span><span class="sxs-lookup"><span data-stu-id="b4837-119">String</span></span>| <span data-ttu-id="b4837-120">导致错误的目录属性的名称。</span><span class="sxs-lookup"><span data-stu-id="b4837-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="b4837-121">当前可能的值： *UserPrincipalName*或*ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="b4837-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="b4837-122">value</span><span class="sxs-lookup"><span data-stu-id="b4837-122">value</span></span>|<span data-ttu-id="b4837-123">String</span><span class="sxs-lookup"><span data-stu-id="b4837-123">String</span></span>| <span data-ttu-id="b4837-124">导致错误的属性的值。</span><span class="sxs-lookup"><span data-stu-id="b4837-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b4837-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4837-125">JSON representation</span></span>
<span data-ttu-id="b4837-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4837-126">Here is a JSON representation of the resource.</span></span>

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
