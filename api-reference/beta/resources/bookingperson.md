---
title: bookingPerson 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: d5ebbd7c4abaf34b31ac3f3d8e75defd6c939ec0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453660"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="4ebbd-104">bookingPerson 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ebbd-104">bookingPerson resource type</span></span>

<span data-ttu-id="4ebbd-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ebbd-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="4ebbd-106">这是 Microsoft 记帐企业中的人员的基本类型，可以是[bookingCustomer](bookingcustomer.md)或[bookingStaffMember](bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="4ebbd-106">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4ebbd-107">属性</span><span class="sxs-lookup"><span data-stu-id="4ebbd-107">Properties</span></span>
| <span data-ttu-id="4ebbd-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ebbd-108">Property</span></span>     | <span data-ttu-id="4ebbd-109">类型</span><span class="sxs-lookup"><span data-stu-id="4ebbd-109">Type</span></span>   |<span data-ttu-id="4ebbd-110">说明</span><span class="sxs-lookup"><span data-stu-id="4ebbd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ebbd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4ebbd-111">displayName</span></span>|<span data-ttu-id="4ebbd-112">字符串</span><span class="sxs-lookup"><span data-stu-id="4ebbd-112">String</span></span>|<span data-ttu-id="4ebbd-113">派生实体的名称，与客户进行交互。</span><span class="sxs-lookup"><span data-stu-id="4ebbd-113">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="4ebbd-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4ebbd-114">emailAddress</span></span>|<span data-ttu-id="4ebbd-115">String</span><span class="sxs-lookup"><span data-stu-id="4ebbd-115">String</span></span>|<span data-ttu-id="4ebbd-116">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="4ebbd-116">The email address of the person.</span></span>|
|<span data-ttu-id="4ebbd-117">id</span><span class="sxs-lookup"><span data-stu-id="4ebbd-117">id</span></span>|<span data-ttu-id="4ebbd-118">String</span><span class="sxs-lookup"><span data-stu-id="4ebbd-118">String</span></span>| <span data-ttu-id="4ebbd-119">派生实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="4ebbd-119">The ID for the derived entity.</span></span> <span data-ttu-id="4ebbd-120">只读。</span><span class="sxs-lookup"><span data-stu-id="4ebbd-120">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ebbd-121">关系</span><span class="sxs-lookup"><span data-stu-id="4ebbd-121">Relationships</span></span>
<span data-ttu-id="4ebbd-122">无</span><span class="sxs-lookup"><span data-stu-id="4ebbd-122">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4ebbd-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ebbd-123">JSON representation</span></span>

<span data-ttu-id="4ebbd-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ebbd-124">The following is a JSON representation of the resource.</span></span>

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
