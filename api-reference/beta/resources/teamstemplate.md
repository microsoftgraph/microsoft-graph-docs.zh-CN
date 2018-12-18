---
title: teamsTemplate 资源类型
description: 介绍 teamsTemplate 实体。
author: nkramer
ms.openlocfilehash: b4e32448f864048fdcb54dc001b21b262df2bba3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327711"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="57593-103">teamsTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="57593-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="57593-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="57593-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57593-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="57593-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="57593-106">工作组模板是在 Microsoft 团队中创建[团队](../resources/team.md)蓝图。</span><span class="sxs-lookup"><span data-stu-id="57593-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="57593-107">模板指定在使用模板创建新团队结构、 设置和偶数应设置的内容。</span><span class="sxs-lookup"><span data-stu-id="57593-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="57593-108">Microsoft 提供了一套基本模板，客户可以节省自己的自定义模板。</span><span class="sxs-lookup"><span data-stu-id="57593-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="57593-109">属性</span><span class="sxs-lookup"><span data-stu-id="57593-109">Properties</span></span>

| <span data-ttu-id="57593-110">属性</span><span class="sxs-lookup"><span data-stu-id="57593-110">Property</span></span>            | <span data-ttu-id="57593-111">类型</span><span class="sxs-lookup"><span data-stu-id="57593-111">Type</span></span>     | <span data-ttu-id="57593-112">说明</span><span class="sxs-lookup"><span data-stu-id="57593-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="57593-113">id</span><span class="sxs-lookup"><span data-stu-id="57593-113">id</span></span>                  | <span data-ttu-id="57593-114">字符串</span><span class="sxs-lookup"><span data-stu-id="57593-114">String</span></span>   | <span data-ttu-id="57593-115">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="57593-115">Unique identifier of the template.</span></span> <span data-ttu-id="57593-116">不能为 null。</span><span class="sxs-lookup"><span data-stu-id="57593-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="57593-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57593-117">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="57593-118">另请参阅</span><span class="sxs-lookup"><span data-stu-id="57593-118">See also</span></span>

- [<span data-ttu-id="57593-119">团队</span><span class="sxs-lookup"><span data-stu-id="57593-119">team</span></span>](team.md)

