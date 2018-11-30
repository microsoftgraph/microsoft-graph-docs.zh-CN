---
title: licenseDetails 资源类型
description: 包含已分配给用户的许可证的相关信息。
ms.openlocfilehash: dd56026d2c1d230fe6bb25b78ff8ababa01f577b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049059"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="3799a-103">licenseDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="3799a-103">licenseDetails resource type</span></span>

> <span data-ttu-id="3799a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3799a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3799a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3799a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3799a-106">包含已分配给用户的许可证的相关信息。</span><span class="sxs-lookup"><span data-stu-id="3799a-106">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="3799a-107">方法</span><span class="sxs-lookup"><span data-stu-id="3799a-107">Methods</span></span>

| <span data-ttu-id="3799a-108">方法</span><span class="sxs-lookup"><span data-stu-id="3799a-108">Method</span></span>           | <span data-ttu-id="3799a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3799a-109">Return Type</span></span>    |<span data-ttu-id="3799a-110">说明</span><span class="sxs-lookup"><span data-stu-id="3799a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3799a-111">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="3799a-111">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="3799a-112">licenseDetails collection</span><span class="sxs-lookup"><span data-stu-id="3799a-112">licenseDetails collection</span></span> |<span data-ttu-id="3799a-113">检索用户的 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="3799a-113">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="3799a-114">属性</span><span class="sxs-lookup"><span data-stu-id="3799a-114">Properties</span></span>
| <span data-ttu-id="3799a-115">属性</span><span class="sxs-lookup"><span data-stu-id="3799a-115">Property</span></span>     | <span data-ttu-id="3799a-116">类型</span><span class="sxs-lookup"><span data-stu-id="3799a-116">Type</span></span>   |<span data-ttu-id="3799a-117">说明</span><span class="sxs-lookup"><span data-stu-id="3799a-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3799a-118">id</span><span class="sxs-lookup"><span data-stu-id="3799a-118">id</span></span>|<span data-ttu-id="3799a-119">String</span><span class="sxs-lookup"><span data-stu-id="3799a-119">String</span></span>| <span data-ttu-id="3799a-p102">许可证详细信息对象的唯一标识符。只读，密钥，不可为 NULL</span><span class="sxs-lookup"><span data-stu-id="3799a-p102">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="3799a-122">servicePlans</span><span class="sxs-lookup"><span data-stu-id="3799a-122">servicePlans</span></span>|<span data-ttu-id="3799a-123">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="3799a-123">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="3799a-p103">许可证分配的服务计划的相关信息。只读，不可为 Null</span><span class="sxs-lookup"><span data-stu-id="3799a-p103">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="3799a-126">skuId</span><span class="sxs-lookup"><span data-stu-id="3799a-126">skuId</span></span>|<span data-ttu-id="3799a-127">Guid</span><span class="sxs-lookup"><span data-stu-id="3799a-127">Guid</span></span>| <span data-ttu-id="3799a-p104">服务 SKU 的唯一标识符 (GUID)。等同于相关的 [SubscribedSku](subscribedsku.md) 对象上的 skuId 属性。只读</span><span class="sxs-lookup"><span data-stu-id="3799a-p104">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="3799a-131">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="3799a-131">skuPartNumber</span></span>|<span data-ttu-id="3799a-132">String</span><span class="sxs-lookup"><span data-stu-id="3799a-132">String</span></span>| <span data-ttu-id="3799a-p105">唯一的 SKU 显示名称。等同于相关的 [SubscribedSku](subscribedsku.md) 对象上的 skuPartNumber；例如：“AAD_Premium”。只读</span><span class="sxs-lookup"><span data-stu-id="3799a-p105">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="3799a-136">关系</span><span class="sxs-lookup"><span data-stu-id="3799a-136">Relationships</span></span>
<span data-ttu-id="3799a-137">无</span><span class="sxs-lookup"><span data-stu-id="3799a-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3799a-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3799a-138">JSON representation</span></span>
<span data-ttu-id="3799a-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3799a-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->