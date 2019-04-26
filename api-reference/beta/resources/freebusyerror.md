---
title: freeBusyError 资源类型
description: 表示尝试获取用户、通讯组列表或资源可用性的错误信息。
localization_priority: Normal
ms.openlocfilehash: e2c755b51e72adf3ff4efa4de5c9438e70d701e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547494"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="49722-103">freeBusyError 资源类型</span><span class="sxs-lookup"><span data-stu-id="49722-103">freeBusyError resource type</span></span>

<span data-ttu-id="49722-104">表示尝试获取用户、通讯组列表或资源可用性的错误信息。</span><span class="sxs-lookup"><span data-stu-id="49722-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="49722-105">属性</span><span class="sxs-lookup"><span data-stu-id="49722-105">Properties</span></span>
| <span data-ttu-id="49722-106">属性</span><span class="sxs-lookup"><span data-stu-id="49722-106">Property</span></span>     | <span data-ttu-id="49722-107">类型</span><span class="sxs-lookup"><span data-stu-id="49722-107">Type</span></span>   |<span data-ttu-id="49722-108">描述</span><span class="sxs-lookup"><span data-stu-id="49722-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49722-109">message</span><span class="sxs-lookup"><span data-stu-id="49722-109">message</span></span> |<span data-ttu-id="49722-110">String</span><span class="sxs-lookup"><span data-stu-id="49722-110">String</span></span> |<span data-ttu-id="49722-111">描述错误。</span><span class="sxs-lookup"><span data-stu-id="49722-111">Describes the error.</span></span> |
|<span data-ttu-id="49722-112">responseCode</span><span class="sxs-lookup"><span data-stu-id="49722-112">responseCode</span></span> |<span data-ttu-id="49722-113">String</span><span class="sxs-lookup"><span data-stu-id="49722-113">String</span></span> |<span data-ttu-id="49722-114">对用户、通讯组列表或资源的可用性进行查询的响应代码。</span><span class="sxs-lookup"><span data-stu-id="49722-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="49722-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49722-115">JSON representation</span></span>

<span data-ttu-id="49722-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49722-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
