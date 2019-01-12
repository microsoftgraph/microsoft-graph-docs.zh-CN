---
title: teamsTemplate 资源类型
description: 介绍 teamsTemplate 实体。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9bd5047950ed1ed3c57950d2c4b708a78b570649
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940083"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="338b7-103">teamsTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="338b7-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="338b7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="338b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="338b7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="338b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="338b7-106">工作组模板是在 Microsoft 团队中创建[团队](../resources/team.md)蓝图。</span><span class="sxs-lookup"><span data-stu-id="338b7-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="338b7-107">模板指定在使用模板创建新团队结构、 设置和偶数应设置的内容。</span><span class="sxs-lookup"><span data-stu-id="338b7-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="338b7-108">Microsoft 提供了一套基本模板，客户可以节省自己的自定义模板。</span><span class="sxs-lookup"><span data-stu-id="338b7-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="338b7-109">属性</span><span class="sxs-lookup"><span data-stu-id="338b7-109">Properties</span></span>

| <span data-ttu-id="338b7-110">属性</span><span class="sxs-lookup"><span data-stu-id="338b7-110">Property</span></span>            | <span data-ttu-id="338b7-111">类型</span><span class="sxs-lookup"><span data-stu-id="338b7-111">Type</span></span>     | <span data-ttu-id="338b7-112">说明</span><span class="sxs-lookup"><span data-stu-id="338b7-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="338b7-113">id</span><span class="sxs-lookup"><span data-stu-id="338b7-113">id</span></span>                  | <span data-ttu-id="338b7-114">字符串</span><span class="sxs-lookup"><span data-stu-id="338b7-114">String</span></span>   | <span data-ttu-id="338b7-115">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="338b7-115">Unique identifier of the template.</span></span> <span data-ttu-id="338b7-116">不能为 null。</span><span class="sxs-lookup"><span data-stu-id="338b7-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="338b7-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="338b7-117">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="338b7-118">另请参阅</span><span class="sxs-lookup"><span data-stu-id="338b7-118">See also</span></span>

- [<span data-ttu-id="338b7-119">团队</span><span class="sxs-lookup"><span data-stu-id="338b7-119">team</span></span>](team.md)

