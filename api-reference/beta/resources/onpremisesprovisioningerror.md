---
title: onPremisesProvisioningError 资源类型
description: 表示在将本地目录同步到 Azure Active directory 时, 用户、组或组织联系人实体的目录同步错误。
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568848"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="02d25-103">onPremisesProvisioningError 资源类型</span><span class="sxs-lookup"><span data-stu-id="02d25-103">onPremisesProvisioningError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02d25-104">表示在将本地目录同步到 Azure Active directory 时,[用户](user.md)、[组](group.md)或[组织联系人](orgcontact.md)实体的目录同步错误。</span><span class="sxs-lookup"><span data-stu-id="02d25-104">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="02d25-105">属性</span><span class="sxs-lookup"><span data-stu-id="02d25-105">Properties</span></span>

| <span data-ttu-id="02d25-106">属性</span><span class="sxs-lookup"><span data-stu-id="02d25-106">Property</span></span> | <span data-ttu-id="02d25-107">类型</span><span class="sxs-lookup"><span data-stu-id="02d25-107">Type</span></span> | <span data-ttu-id="02d25-108">说明</span><span class="sxs-lookup"><span data-stu-id="02d25-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="02d25-109">category</span><span class="sxs-lookup"><span data-stu-id="02d25-109">category</span></span>|<span data-ttu-id="02d25-110">String</span><span class="sxs-lookup"><span data-stu-id="02d25-110">String</span></span>| <span data-ttu-id="02d25-111">设置错误的类别。</span><span class="sxs-lookup"><span data-stu-id="02d25-111">Category of the provisioning error.</span></span> <span data-ttu-id="02d25-112">注意: 目前, 只有一个可能的值。</span><span class="sxs-lookup"><span data-stu-id="02d25-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="02d25-113">可能的值: *PropertyConflict* -指示属性值不是唯一的。</span><span class="sxs-lookup"><span data-stu-id="02d25-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="02d25-114">其他对象包含相同的属性值。</span><span class="sxs-lookup"><span data-stu-id="02d25-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="02d25-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="02d25-115">occurredDateTime</span></span>|<span data-ttu-id="02d25-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02d25-116">DateTimeOffset</span></span>| <span data-ttu-id="02d25-117">发生错误的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="02d25-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="02d25-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="02d25-118">propertyCausingError</span></span>|<span data-ttu-id="02d25-119">String</span><span class="sxs-lookup"><span data-stu-id="02d25-119">String</span></span>| <span data-ttu-id="02d25-120">导致错误的目录属性的名称。</span><span class="sxs-lookup"><span data-stu-id="02d25-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="02d25-121">当前可能的值: *UserPrincipalName*或*ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="02d25-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="02d25-122">value</span><span class="sxs-lookup"><span data-stu-id="02d25-122">value</span></span>|<span data-ttu-id="02d25-123">String</span><span class="sxs-lookup"><span data-stu-id="02d25-123">String</span></span>| <span data-ttu-id="02d25-124">导致错误的属性的值。</span><span class="sxs-lookup"><span data-stu-id="02d25-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02d25-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02d25-125">JSON representation</span></span>
<span data-ttu-id="02d25-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02d25-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesprovisioningerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
