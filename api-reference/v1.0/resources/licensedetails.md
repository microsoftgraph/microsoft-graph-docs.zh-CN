---
title: licenseDetails 资源类型
description: 包含已分配给用户的许可证的相关信息。
ms.openlocfilehash: 8c357617eea04151851a0e3a27c41937abd07b28
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009189"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="0fd2e-103">licenseDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fd2e-103">licenseDetails resource type</span></span>

<span data-ttu-id="0fd2e-104">包含已分配给用户的许可证的相关信息。</span><span class="sxs-lookup"><span data-stu-id="0fd2e-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="0fd2e-105">方法</span><span class="sxs-lookup"><span data-stu-id="0fd2e-105">Methods</span></span>

| <span data-ttu-id="0fd2e-106">方法</span><span class="sxs-lookup"><span data-stu-id="0fd2e-106">Method</span></span>           | <span data-ttu-id="0fd2e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fd2e-107">Return Type</span></span>    |<span data-ttu-id="0fd2e-108">说明</span><span class="sxs-lookup"><span data-stu-id="0fd2e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0fd2e-109">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="0fd2e-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="0fd2e-110">licenseDetails collection</span><span class="sxs-lookup"><span data-stu-id="0fd2e-110">licenseDetails collection</span></span> |<span data-ttu-id="0fd2e-111">检索用户的 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="0fd2e-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="0fd2e-112">属性</span><span class="sxs-lookup"><span data-stu-id="0fd2e-112">Properties</span></span>
| <span data-ttu-id="0fd2e-113">属性</span><span class="sxs-lookup"><span data-stu-id="0fd2e-113">Property</span></span>     | <span data-ttu-id="0fd2e-114">类型</span><span class="sxs-lookup"><span data-stu-id="0fd2e-114">Type</span></span>   |<span data-ttu-id="0fd2e-115">说明</span><span class="sxs-lookup"><span data-stu-id="0fd2e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fd2e-116">id</span><span class="sxs-lookup"><span data-stu-id="0fd2e-116">id</span></span>|<span data-ttu-id="0fd2e-117">String</span><span class="sxs-lookup"><span data-stu-id="0fd2e-117">String</span></span>| <span data-ttu-id="0fd2e-p101">许可证详细信息对象的唯一标识符。只读，密钥，不可为 NULL</span><span class="sxs-lookup"><span data-stu-id="0fd2e-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="0fd2e-120">servicePlans</span><span class="sxs-lookup"><span data-stu-id="0fd2e-120">servicePlans</span></span>|<span data-ttu-id="0fd2e-121">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="0fd2e-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="0fd2e-p102">许可证分配的服务计划的相关信息。只读，不可为 Null</span><span class="sxs-lookup"><span data-stu-id="0fd2e-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="0fd2e-124">skuId</span><span class="sxs-lookup"><span data-stu-id="0fd2e-124">skuId</span></span>|<span data-ttu-id="0fd2e-125">Guid</span><span class="sxs-lookup"><span data-stu-id="0fd2e-125">Guid</span></span>| <span data-ttu-id="0fd2e-p103">服务 SKU 的唯一标识符 (GUID)。等同于相关的 [SubscribedSku](subscribedsku.md) 对象上的 skuId 属性。只读</span><span class="sxs-lookup"><span data-stu-id="0fd2e-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="0fd2e-129">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="0fd2e-129">skuPartNumber</span></span>|<span data-ttu-id="0fd2e-130">String</span><span class="sxs-lookup"><span data-stu-id="0fd2e-130">String</span></span>| <span data-ttu-id="0fd2e-p104">唯一的 SKU 显示名称。等同于相关的 [SubscribedSku](subscribedsku.md) 对象上的 skuPartNumber；例如：“AAD_Premium”。只读</span><span class="sxs-lookup"><span data-stu-id="0fd2e-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="0fd2e-134">关系</span><span class="sxs-lookup"><span data-stu-id="0fd2e-134">Relationships</span></span>
<span data-ttu-id="0fd2e-135">无</span><span class="sxs-lookup"><span data-stu-id="0fd2e-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fd2e-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fd2e-136">JSON representation</span></span>
<span data-ttu-id="0fd2e-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fd2e-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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