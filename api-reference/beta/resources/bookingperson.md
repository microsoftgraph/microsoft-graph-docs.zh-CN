---
title: bookingPerson 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: be00e59e2378c454cd9c939f992376dd9c54c3b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543777"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="9e673-104">bookingPerson 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e673-104">bookingPerson resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="9e673-105">这是 Microsoft 记帐企业中的人员的基本类型, 可以是[bookingCustomer](bookingcustomer.md)或[bookingStaffMember](bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="9e673-105">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9e673-106">属性</span><span class="sxs-lookup"><span data-stu-id="9e673-106">Properties</span></span>
| <span data-ttu-id="9e673-107">属性</span><span class="sxs-lookup"><span data-stu-id="9e673-107">Property</span></span>     | <span data-ttu-id="9e673-108">类型</span><span class="sxs-lookup"><span data-stu-id="9e673-108">Type</span></span>   |<span data-ttu-id="9e673-109">说明</span><span class="sxs-lookup"><span data-stu-id="9e673-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e673-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9e673-110">displayName</span></span>|<span data-ttu-id="9e673-111">字符串</span><span class="sxs-lookup"><span data-stu-id="9e673-111">String</span></span>|<span data-ttu-id="9e673-112">派生实体的名称, 与客户进行交互。</span><span class="sxs-lookup"><span data-stu-id="9e673-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="9e673-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9e673-113">emailAddress</span></span>|<span data-ttu-id="9e673-114">String</span><span class="sxs-lookup"><span data-stu-id="9e673-114">String</span></span>|<span data-ttu-id="9e673-115">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9e673-115">The email address of the person.</span></span>|
|<span data-ttu-id="9e673-116">id</span><span class="sxs-lookup"><span data-stu-id="9e673-116">id</span></span>|<span data-ttu-id="9e673-117">String</span><span class="sxs-lookup"><span data-stu-id="9e673-117">String</span></span>| <span data-ttu-id="9e673-118">派生实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="9e673-118">The ID for the derived entity.</span></span> <span data-ttu-id="9e673-119">只读。</span><span class="sxs-lookup"><span data-stu-id="9e673-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e673-120">关系</span><span class="sxs-lookup"><span data-stu-id="9e673-120">Relationships</span></span>
<span data-ttu-id="9e673-121">无</span><span class="sxs-lookup"><span data-stu-id="9e673-121">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9e673-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e673-122">JSON representation</span></span>

<span data-ttu-id="9e673-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e673-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingPerson"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingperson.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
