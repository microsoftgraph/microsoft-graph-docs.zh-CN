---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
ms.openlocfilehash: 5085c144045631c530cbb66f5e1f27186a63b380
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513646"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="a5879-103">informationalUrl 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5879-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5879-104">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="a5879-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="a5879-105">属性</span><span class="sxs-lookup"><span data-stu-id="a5879-105">Properties</span></span>

| <span data-ttu-id="a5879-106">属性</span><span class="sxs-lookup"><span data-stu-id="a5879-106">Property</span></span> | <span data-ttu-id="a5879-107">类型</span><span class="sxs-lookup"><span data-stu-id="a5879-107">Type</span></span> | <span data-ttu-id="a5879-108">说明</span><span class="sxs-lookup"><span data-stu-id="a5879-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a5879-109">市场营销</span><span class="sxs-lookup"><span data-stu-id="a5879-109">marketing</span></span>|<span data-ttu-id="a5879-110">String</span><span class="sxs-lookup"><span data-stu-id="a5879-110">String</span></span>| <span data-ttu-id="a5879-111">链接到应用程序的市场营销页。</span><span class="sxs-lookup"><span data-stu-id="a5879-111">Link to the application's marketing page.</span></span> <span data-ttu-id="a5879-112">例如，https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="a5879-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="a5879-113">隐私</span><span class="sxs-lookup"><span data-stu-id="a5879-113">privacy</span></span>|<span data-ttu-id="a5879-114">String</span><span class="sxs-lookup"><span data-stu-id="a5879-114">String</span></span>| <span data-ttu-id="a5879-115">链接到应用程序的隐私声明。</span><span class="sxs-lookup"><span data-stu-id="a5879-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="a5879-116">例如，https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="a5879-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="a5879-117">支持</span><span class="sxs-lookup"><span data-stu-id="a5879-117">support</span></span>|<span data-ttu-id="a5879-118">String</span><span class="sxs-lookup"><span data-stu-id="a5879-118">String</span></span>| <span data-ttu-id="a5879-119">链接到应用程序的支持网页。</span><span class="sxs-lookup"><span data-stu-id="a5879-119">Link to the application's support page.</span></span> <span data-ttu-id="a5879-120">例如，https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="a5879-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="a5879-121">termsOfService</span><span class="sxs-lookup"><span data-stu-id="a5879-121">termsOfService</span></span>|<span data-ttu-id="a5879-122">String</span><span class="sxs-lookup"><span data-stu-id="a5879-122">String</span></span>| <span data-ttu-id="a5879-123">链接到的服务语句的应用程序的术语。</span><span class="sxs-lookup"><span data-stu-id="a5879-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="a5879-124">例如，https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="a5879-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a5879-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5879-125">JSON representation</span></span>
<span data-ttu-id="a5879-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5879-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/informationalurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
