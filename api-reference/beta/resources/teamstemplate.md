---
title: teamsTemplate 资源类型
description: 介绍 teamsTemplate 实体。
ms.openlocfilehash: 76b2921e884d38a57097789b1ba64df3309d141c
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2018
ms.locfileid: "27210137"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="cd010-103">teamsTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd010-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="cd010-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cd010-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd010-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cd010-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd010-106">工作组模板是在 Microsoft 团队中创建[团队](../resources/team.md)蓝图。</span><span class="sxs-lookup"><span data-stu-id="cd010-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="cd010-107">模板指定在使用模板创建新团队结构、 设置和偶数应设置的内容。</span><span class="sxs-lookup"><span data-stu-id="cd010-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="cd010-108">Microsoft 提供了一套基本模板，客户可以节省自己的自定义模板。</span><span class="sxs-lookup"><span data-stu-id="cd010-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="cd010-109">属性</span><span class="sxs-lookup"><span data-stu-id="cd010-109">Properties</span></span>

| <span data-ttu-id="cd010-110">属性</span><span class="sxs-lookup"><span data-stu-id="cd010-110">Property</span></span>            | <span data-ttu-id="cd010-111">类型</span><span class="sxs-lookup"><span data-stu-id="cd010-111">Type</span></span>     | <span data-ttu-id="cd010-112">说明</span><span class="sxs-lookup"><span data-stu-id="cd010-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="cd010-113">id</span><span class="sxs-lookup"><span data-stu-id="cd010-113">id</span></span>                  | <span data-ttu-id="cd010-114">字符串</span><span class="sxs-lookup"><span data-stu-id="cd010-114">String</span></span>   | <span data-ttu-id="cd010-115">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cd010-115">Unique identifier of the template.</span></span> <span data-ttu-id="cd010-116">不能为 null。</span><span class="sxs-lookup"><span data-stu-id="cd010-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cd010-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd010-117">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a><span data-ttu-id="cd010-118">另请参阅</span><span class="sxs-lookup"><span data-stu-id="cd010-118">See also</span></span>

- [<span data-ttu-id="cd010-119">团队</span><span class="sxs-lookup"><span data-stu-id="cd010-119">team</span></span>](team.md)

