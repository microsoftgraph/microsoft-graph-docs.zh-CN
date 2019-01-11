---
title: onPremisesProvisioningError 资源类型
description: 同步到 Azure Active Directory 的内部部署目录时，表示为用户和组的实体的目录同步错误。
localization_priority: Normal
ms.openlocfilehash: c8989a78dfb60a6c7c25a66a9f1e619dcbdca15d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830665"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="3e255-103">onPremisesProvisioningError 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e255-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="3e255-104">时同步部署到 Azure Active Directory 目录，则表示[用户](user.md)和[组](group.md)实体的目录同步错误。</span><span class="sxs-lookup"><span data-stu-id="3e255-104">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="3e255-105">属性</span><span class="sxs-lookup"><span data-stu-id="3e255-105">Properties</span></span>

| <span data-ttu-id="3e255-106">属性</span><span class="sxs-lookup"><span data-stu-id="3e255-106">Property</span></span> | <span data-ttu-id="3e255-107">类型</span><span class="sxs-lookup"><span data-stu-id="3e255-107">Type</span></span> | <span data-ttu-id="3e255-108">说明</span><span class="sxs-lookup"><span data-stu-id="3e255-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3e255-109">category</span><span class="sxs-lookup"><span data-stu-id="3e255-109">category</span></span>|<span data-ttu-id="3e255-110">String</span><span class="sxs-lookup"><span data-stu-id="3e255-110">String</span></span>| <span data-ttu-id="3e255-111">设置错误的类别。</span><span class="sxs-lookup"><span data-stu-id="3e255-111">Category of the provisioning error.</span></span> <span data-ttu-id="3e255-112">注意： 当前，没有只有一个可能的值。</span><span class="sxs-lookup"><span data-stu-id="3e255-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="3e255-113">可能的值： *PropertyConflict* -指示属性值不唯一。</span><span class="sxs-lookup"><span data-stu-id="3e255-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="3e255-114">其他对象包含的属性相同的值。</span><span class="sxs-lookup"><span data-stu-id="3e255-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="3e255-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="3e255-115">occurredDateTime</span></span>|<span data-ttu-id="3e255-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e255-116">DateTimeOffset</span></span>| <span data-ttu-id="3e255-117">日期和时间发生错误。</span><span class="sxs-lookup"><span data-stu-id="3e255-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="3e255-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="3e255-118">propertyCausingError</span></span>|<span data-ttu-id="3e255-119">字符串</span><span class="sxs-lookup"><span data-stu-id="3e255-119">String</span></span>| <span data-ttu-id="3e255-120">导致此错误的目录属性的名称。</span><span class="sxs-lookup"><span data-stu-id="3e255-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="3e255-121">当前的可能值： *UserPrincipalName*或*ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="3e255-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="3e255-122">值</span><span class="sxs-lookup"><span data-stu-id="3e255-122">value</span></span>|<span data-ttu-id="3e255-123">字符串</span><span class="sxs-lookup"><span data-stu-id="3e255-123">String</span></span>| <span data-ttu-id="3e255-124">导致错误属性的值。</span><span class="sxs-lookup"><span data-stu-id="3e255-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3e255-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e255-125">JSON representation</span></span>
<span data-ttu-id="3e255-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e255-126">Here is a JSON representation of the resource.</span></span>

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
