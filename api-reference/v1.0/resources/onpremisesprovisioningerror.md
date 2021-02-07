---
title: onPremisesProvisioningError 资源类型
description: 表示将本地目录同步到 Azure Active Directory 时用户组和联系人资源的目录同步错误。
localization_priority: Normal
author: japere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2647e32653d26793b4f875bb47ce43e83a294c4a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133328"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="62358-103">onPremisesProvisioningError 资源类型</span><span class="sxs-lookup"><span data-stu-id="62358-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="62358-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62358-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62358-105">表示将本地目录同步到[](user.md)Azure [](group.md) Active Directory 时用户、组和[orgContact](orgcontact.md)资源的目录同步错误。</span><span class="sxs-lookup"><span data-stu-id="62358-105">Represents directory synchronization errors for the [user](user.md), [group](group.md) and [orgContact](orgcontact.md) resources when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="62358-106">属性</span><span class="sxs-lookup"><span data-stu-id="62358-106">Properties</span></span>

| <span data-ttu-id="62358-107">属性</span><span class="sxs-lookup"><span data-stu-id="62358-107">Property</span></span> | <span data-ttu-id="62358-108">类型</span><span class="sxs-lookup"><span data-stu-id="62358-108">Type</span></span> | <span data-ttu-id="62358-109">说明</span><span class="sxs-lookup"><span data-stu-id="62358-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="62358-110">“类别”</span><span class="sxs-lookup"><span data-stu-id="62358-110">category</span></span>|<span data-ttu-id="62358-111">String</span><span class="sxs-lookup"><span data-stu-id="62358-111">String</span></span>| <span data-ttu-id="62358-112">设置错误的类别。</span><span class="sxs-lookup"><span data-stu-id="62358-112">Category of the provisioning error.</span></span> <span data-ttu-id="62358-113">注意：目前只有一个可能的值。</span><span class="sxs-lookup"><span data-stu-id="62358-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="62358-114">可能的值 *：PropertyConflict* - 指示属性值不唯一。</span><span class="sxs-lookup"><span data-stu-id="62358-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="62358-115">其他对象包含与属性相同的值。</span><span class="sxs-lookup"><span data-stu-id="62358-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="62358-116">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="62358-116">occurredDateTime</span></span>|<span data-ttu-id="62358-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62358-117">DateTimeOffset</span></span>| <span data-ttu-id="62358-118">发生错误的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="62358-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="62358-119">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="62358-119">propertyCausingError</span></span>|<span data-ttu-id="62358-120">String</span><span class="sxs-lookup"><span data-stu-id="62358-120">String</span></span>| <span data-ttu-id="62358-121">导致错误的目录属性的名称。</span><span class="sxs-lookup"><span data-stu-id="62358-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="62358-122">当前可能的值 *：UserPrincipalName* 或 *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="62358-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="62358-123">value</span><span class="sxs-lookup"><span data-stu-id="62358-123">value</span></span>|<span data-ttu-id="62358-124">String</span><span class="sxs-lookup"><span data-stu-id="62358-124">String</span></span>| <span data-ttu-id="62358-125">导致错误的属性值。</span><span class="sxs-lookup"><span data-stu-id="62358-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="62358-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62358-126">JSON representation</span></span>
<span data-ttu-id="62358-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62358-127">Here is a JSON representation of the resource.</span></span>

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

