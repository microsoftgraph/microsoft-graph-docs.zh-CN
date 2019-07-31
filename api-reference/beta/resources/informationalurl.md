---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9e2eaad003f4669623a4db4af1b364e05198515d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006253"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="82a06-103">informationalUrl 资源类型</span><span class="sxs-lookup"><span data-stu-id="82a06-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82a06-104">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="82a06-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="82a06-105">属性</span><span class="sxs-lookup"><span data-stu-id="82a06-105">Properties</span></span>

| <span data-ttu-id="82a06-106">属性</span><span class="sxs-lookup"><span data-stu-id="82a06-106">Property</span></span> | <span data-ttu-id="82a06-107">类型</span><span class="sxs-lookup"><span data-stu-id="82a06-107">Type</span></span> | <span data-ttu-id="82a06-108">说明</span><span class="sxs-lookup"><span data-stu-id="82a06-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="82a06-109">部门</span><span class="sxs-lookup"><span data-stu-id="82a06-109">marketing</span></span>|<span data-ttu-id="82a06-110">String</span><span class="sxs-lookup"><span data-stu-id="82a06-110">String</span></span>| <span data-ttu-id="82a06-111">指向应用程序的市场营销页面的链接。</span><span class="sxs-lookup"><span data-stu-id="82a06-111">Link to the application's marketing page.</span></span> <span data-ttu-id="82a06-112">例如，https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="82a06-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="82a06-113">私密性</span><span class="sxs-lookup"><span data-stu-id="82a06-113">privacy</span></span>|<span data-ttu-id="82a06-114">String</span><span class="sxs-lookup"><span data-stu-id="82a06-114">String</span></span>| <span data-ttu-id="82a06-115">指向应用程序的隐私声明的链接。</span><span class="sxs-lookup"><span data-stu-id="82a06-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="82a06-116">例如，https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="82a06-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="82a06-117">支持</span><span class="sxs-lookup"><span data-stu-id="82a06-117">support</span></span>|<span data-ttu-id="82a06-118">String</span><span class="sxs-lookup"><span data-stu-id="82a06-118">String</span></span>| <span data-ttu-id="82a06-119">指向应用程序的支持页的链接。</span><span class="sxs-lookup"><span data-stu-id="82a06-119">Link to the application's support page.</span></span> <span data-ttu-id="82a06-120">例如，https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="82a06-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="82a06-121">termsOfService</span><span class="sxs-lookup"><span data-stu-id="82a06-121">termsOfService</span></span>|<span data-ttu-id="82a06-122">String</span><span class="sxs-lookup"><span data-stu-id="82a06-122">String</span></span>| <span data-ttu-id="82a06-123">指向应用程序的服务条款声明的链接。</span><span class="sxs-lookup"><span data-stu-id="82a06-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="82a06-124">例如，https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="82a06-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="82a06-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82a06-125">JSON representation</span></span>
<span data-ttu-id="82a06-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82a06-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
