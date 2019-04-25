---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
ms.openlocfilehash: 5085c144045631c530cbb66f5e1f27186a63b380
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548703"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="a85c8-103">informationalUrl 资源类型</span><span class="sxs-lookup"><span data-stu-id="a85c8-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a85c8-104">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="a85c8-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="a85c8-105">属性</span><span class="sxs-lookup"><span data-stu-id="a85c8-105">Properties</span></span>

| <span data-ttu-id="a85c8-106">属性</span><span class="sxs-lookup"><span data-stu-id="a85c8-106">Property</span></span> | <span data-ttu-id="a85c8-107">类型</span><span class="sxs-lookup"><span data-stu-id="a85c8-107">Type</span></span> | <span data-ttu-id="a85c8-108">说明</span><span class="sxs-lookup"><span data-stu-id="a85c8-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a85c8-109">部门</span><span class="sxs-lookup"><span data-stu-id="a85c8-109">marketing</span></span>|<span data-ttu-id="a85c8-110">String</span><span class="sxs-lookup"><span data-stu-id="a85c8-110">String</span></span>| <span data-ttu-id="a85c8-111">指向应用程序的市场营销页面的链接。</span><span class="sxs-lookup"><span data-stu-id="a85c8-111">Link to the application's marketing page.</span></span> <span data-ttu-id="a85c8-112">例如，https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="a85c8-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="a85c8-113">私密性</span><span class="sxs-lookup"><span data-stu-id="a85c8-113">privacy</span></span>|<span data-ttu-id="a85c8-114">String</span><span class="sxs-lookup"><span data-stu-id="a85c8-114">String</span></span>| <span data-ttu-id="a85c8-115">指向应用程序的隐私声明的链接。</span><span class="sxs-lookup"><span data-stu-id="a85c8-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="a85c8-116">例如，https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="a85c8-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="a85c8-117">支持</span><span class="sxs-lookup"><span data-stu-id="a85c8-117">support</span></span>|<span data-ttu-id="a85c8-118">String</span><span class="sxs-lookup"><span data-stu-id="a85c8-118">String</span></span>| <span data-ttu-id="a85c8-119">指向应用程序的支持页的链接。</span><span class="sxs-lookup"><span data-stu-id="a85c8-119">Link to the application's support page.</span></span> <span data-ttu-id="a85c8-120">例如，https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="a85c8-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="a85c8-121">termsOfService</span><span class="sxs-lookup"><span data-stu-id="a85c8-121">termsOfService</span></span>|<span data-ttu-id="a85c8-122">String</span><span class="sxs-lookup"><span data-stu-id="a85c8-122">String</span></span>| <span data-ttu-id="a85c8-123">指向应用程序的服务条款声明的链接。</span><span class="sxs-lookup"><span data-stu-id="a85c8-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="a85c8-124">例如，https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="a85c8-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a85c8-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a85c8-125">JSON representation</span></span>
<span data-ttu-id="a85c8-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a85c8-126">Here is a JSON representation of the resource.</span></span>

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
