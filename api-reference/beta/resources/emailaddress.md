---
title: emailAddress 资源类型
description: 表示的名称和 SMTP 地址的实体实例，例如，邮件收件人或日历所有者。
localization_priority: Normal
ms.openlocfilehash: 5286334378aa5d208cf171ecab0bdc1777a4073b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871223"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="2db06-103">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="2db06-103">emailAddress resource type</span></span>

> <span data-ttu-id="2db06-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2db06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2db06-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2db06-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2db06-106">表示的名称和 SMTP 地址的实体实例，例如，邮件收件人或日历所有者。</span><span class="sxs-lookup"><span data-stu-id="2db06-106">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="2db06-107">属性</span><span class="sxs-lookup"><span data-stu-id="2db06-107">Properties</span></span>
| <span data-ttu-id="2db06-108">属性</span><span class="sxs-lookup"><span data-stu-id="2db06-108">Property</span></span>     | <span data-ttu-id="2db06-109">类型</span><span class="sxs-lookup"><span data-stu-id="2db06-109">Type</span></span>   |<span data-ttu-id="2db06-110">说明</span><span class="sxs-lookup"><span data-stu-id="2db06-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2db06-111">address</span><span class="sxs-lookup"><span data-stu-id="2db06-111">address</span></span>|<span data-ttu-id="2db06-112">String</span><span class="sxs-lookup"><span data-stu-id="2db06-112">String</span></span>|<span data-ttu-id="2db06-113">实体实例的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="2db06-113">The email address of an entity instance.</span></span>|
|<span data-ttu-id="2db06-114">name</span><span class="sxs-lookup"><span data-stu-id="2db06-114">name</span></span>|<span data-ttu-id="2db06-115">字符串</span><span class="sxs-lookup"><span data-stu-id="2db06-115">String</span></span>|<span data-ttu-id="2db06-116">实体实例的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2db06-116">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2db06-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2db06-117">JSON representation</span></span>

<span data-ttu-id="2db06-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2db06-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
