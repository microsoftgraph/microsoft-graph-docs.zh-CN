---
title: onPremisesProvisioningError 资源类型
description: 当同步部署到 Azure Active Directory 目录，则表示用户、 组或组织的 contact 实体的目录同步错误。
localization_priority: Normal
ms.openlocfilehash: 1ea9efcd4d9db5cf7cc5b8f0a18b35345d06c3fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817736"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="6a876-103">onPremisesProvisioningError 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a876-103">onPremisesProvisioningError resource type</span></span>

> <span data-ttu-id="6a876-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a876-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a876-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a876-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a876-106">当同步部署到 Azure Active Directory 目录，则表示[用户](user.md)、[组](group.md)或[组织的联系人](orgcontact.md)实体的目录同步错误。</span><span class="sxs-lookup"><span data-stu-id="6a876-106">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="6a876-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a876-107">Properties</span></span>

| <span data-ttu-id="6a876-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a876-108">Property</span></span> | <span data-ttu-id="6a876-109">类型</span><span class="sxs-lookup"><span data-stu-id="6a876-109">Type</span></span> | <span data-ttu-id="6a876-110">说明</span><span class="sxs-lookup"><span data-stu-id="6a876-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6a876-111">category</span><span class="sxs-lookup"><span data-stu-id="6a876-111">category</span></span>|<span data-ttu-id="6a876-112">String</span><span class="sxs-lookup"><span data-stu-id="6a876-112">String</span></span>| <span data-ttu-id="6a876-113">设置错误的类别。</span><span class="sxs-lookup"><span data-stu-id="6a876-113">Category of the provisioning error.</span></span> <span data-ttu-id="6a876-114">注意： 当前，没有只有一个可能的值。</span><span class="sxs-lookup"><span data-stu-id="6a876-114">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="6a876-115">可能的值： *PropertyConflict* -指示属性值不唯一。</span><span class="sxs-lookup"><span data-stu-id="6a876-115">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="6a876-116">其他对象包含的属性相同的值。</span><span class="sxs-lookup"><span data-stu-id="6a876-116">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="6a876-117">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="6a876-117">occurredDateTime</span></span>|<span data-ttu-id="6a876-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a876-118">DateTimeOffset</span></span>| <span data-ttu-id="6a876-119">日期和时间发生错误。</span><span class="sxs-lookup"><span data-stu-id="6a876-119">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="6a876-120">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="6a876-120">propertyCausingError</span></span>|<span data-ttu-id="6a876-121">字符串</span><span class="sxs-lookup"><span data-stu-id="6a876-121">String</span></span>| <span data-ttu-id="6a876-122">导致此错误的目录属性的名称。</span><span class="sxs-lookup"><span data-stu-id="6a876-122">Name of the directory property causing the error.</span></span> <span data-ttu-id="6a876-123">当前的可能值： *UserPrincipalName*或*ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="6a876-123">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="6a876-124">值</span><span class="sxs-lookup"><span data-stu-id="6a876-124">value</span></span>|<span data-ttu-id="6a876-125">字符串</span><span class="sxs-lookup"><span data-stu-id="6a876-125">String</span></span>| <span data-ttu-id="6a876-126">导致错误属性的值。</span><span class="sxs-lookup"><span data-stu-id="6a876-126">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6a876-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a876-127">JSON representation</span></span>
<span data-ttu-id="6a876-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a876-128">Here is a JSON representation of the resource.</span></span>

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
