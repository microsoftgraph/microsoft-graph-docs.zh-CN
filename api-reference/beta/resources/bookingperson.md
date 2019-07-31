---
title: bookingPerson 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3c8db7aca957878247193207e00e969d8ddfc98e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974162"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="176fe-104">bookingPerson 资源类型</span><span class="sxs-lookup"><span data-stu-id="176fe-104">bookingPerson resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="176fe-105">这是 Microsoft 记帐企业中的人员的基本类型, 可以是[bookingCustomer](bookingcustomer.md)或[bookingStaffMember](bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="176fe-105">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="176fe-106">属性</span><span class="sxs-lookup"><span data-stu-id="176fe-106">Properties</span></span>
| <span data-ttu-id="176fe-107">属性</span><span class="sxs-lookup"><span data-stu-id="176fe-107">Property</span></span>     | <span data-ttu-id="176fe-108">类型</span><span class="sxs-lookup"><span data-stu-id="176fe-108">Type</span></span>   |<span data-ttu-id="176fe-109">说明</span><span class="sxs-lookup"><span data-stu-id="176fe-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="176fe-110">displayName</span><span class="sxs-lookup"><span data-stu-id="176fe-110">displayName</span></span>|<span data-ttu-id="176fe-111">字符串</span><span class="sxs-lookup"><span data-stu-id="176fe-111">String</span></span>|<span data-ttu-id="176fe-112">派生实体的名称, 与客户进行交互。</span><span class="sxs-lookup"><span data-stu-id="176fe-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="176fe-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="176fe-113">emailAddress</span></span>|<span data-ttu-id="176fe-114">String</span><span class="sxs-lookup"><span data-stu-id="176fe-114">String</span></span>|<span data-ttu-id="176fe-115">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="176fe-115">The email address of the person.</span></span>|
|<span data-ttu-id="176fe-116">id</span><span class="sxs-lookup"><span data-stu-id="176fe-116">id</span></span>|<span data-ttu-id="176fe-117">String</span><span class="sxs-lookup"><span data-stu-id="176fe-117">String</span></span>| <span data-ttu-id="176fe-118">派生实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="176fe-118">The ID for the derived entity.</span></span> <span data-ttu-id="176fe-119">只读。</span><span class="sxs-lookup"><span data-stu-id="176fe-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="176fe-120">关系</span><span class="sxs-lookup"><span data-stu-id="176fe-120">Relationships</span></span>
<span data-ttu-id="176fe-121">无</span><span class="sxs-lookup"><span data-stu-id="176fe-121">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="176fe-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="176fe-122">JSON representation</span></span>

<span data-ttu-id="176fe-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="176fe-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
