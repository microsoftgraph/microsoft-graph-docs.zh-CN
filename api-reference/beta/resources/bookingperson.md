---
title: bookingPerson 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b4f69fde11ce0717e7ac81bd2070d08cbb59a84a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338752"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="88a51-104">bookingPerson 资源类型</span><span class="sxs-lookup"><span data-stu-id="88a51-104">bookingPerson resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="88a51-105">这是 Microsoft 记帐企业中的人员的基本类型, 可以是[bookingCustomer](bookingcustomer.md)或[bookingStaffMember](bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="88a51-105">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="88a51-106">属性</span><span class="sxs-lookup"><span data-stu-id="88a51-106">Properties</span></span>
| <span data-ttu-id="88a51-107">属性</span><span class="sxs-lookup"><span data-stu-id="88a51-107">Property</span></span>     | <span data-ttu-id="88a51-108">类型</span><span class="sxs-lookup"><span data-stu-id="88a51-108">Type</span></span>   |<span data-ttu-id="88a51-109">说明</span><span class="sxs-lookup"><span data-stu-id="88a51-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88a51-110">displayName</span><span class="sxs-lookup"><span data-stu-id="88a51-110">displayName</span></span>|<span data-ttu-id="88a51-111">字符串</span><span class="sxs-lookup"><span data-stu-id="88a51-111">String</span></span>|<span data-ttu-id="88a51-112">派生实体的名称, 与客户进行交互。</span><span class="sxs-lookup"><span data-stu-id="88a51-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="88a51-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="88a51-113">emailAddress</span></span>|<span data-ttu-id="88a51-114">String</span><span class="sxs-lookup"><span data-stu-id="88a51-114">String</span></span>|<span data-ttu-id="88a51-115">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="88a51-115">The email address of the person.</span></span>|
|<span data-ttu-id="88a51-116">id</span><span class="sxs-lookup"><span data-stu-id="88a51-116">id</span></span>|<span data-ttu-id="88a51-117">String</span><span class="sxs-lookup"><span data-stu-id="88a51-117">String</span></span>| <span data-ttu-id="88a51-118">派生实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="88a51-118">The ID for the derived entity.</span></span> <span data-ttu-id="88a51-119">只读。</span><span class="sxs-lookup"><span data-stu-id="88a51-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88a51-120">关系</span><span class="sxs-lookup"><span data-stu-id="88a51-120">Relationships</span></span>
<span data-ttu-id="88a51-121">无</span><span class="sxs-lookup"><span data-stu-id="88a51-121">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="88a51-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88a51-122">JSON representation</span></span>

<span data-ttu-id="88a51-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88a51-123">The following is a JSON representation of the resource.</span></span>

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
