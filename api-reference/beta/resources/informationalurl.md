---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
ms.openlocfilehash: c858bb55db083510661edfc36f32b9a511c5e6f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339988"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="8ad55-103">informationalUrl 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ad55-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ad55-104">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="8ad55-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="8ad55-105">属性</span><span class="sxs-lookup"><span data-stu-id="8ad55-105">Properties</span></span>

| <span data-ttu-id="8ad55-106">属性</span><span class="sxs-lookup"><span data-stu-id="8ad55-106">Property</span></span> | <span data-ttu-id="8ad55-107">类型</span><span class="sxs-lookup"><span data-stu-id="8ad55-107">Type</span></span> | <span data-ttu-id="8ad55-108">说明</span><span class="sxs-lookup"><span data-stu-id="8ad55-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8ad55-109">部门</span><span class="sxs-lookup"><span data-stu-id="8ad55-109">marketing</span></span>|<span data-ttu-id="8ad55-110">String</span><span class="sxs-lookup"><span data-stu-id="8ad55-110">String</span></span>| <span data-ttu-id="8ad55-111">指向应用程序的市场营销页面的链接。</span><span class="sxs-lookup"><span data-stu-id="8ad55-111">Link to the application's marketing page.</span></span> <span data-ttu-id="8ad55-112">例如，https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="8ad55-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="8ad55-113">私密性</span><span class="sxs-lookup"><span data-stu-id="8ad55-113">privacy</span></span>|<span data-ttu-id="8ad55-114">String</span><span class="sxs-lookup"><span data-stu-id="8ad55-114">String</span></span>| <span data-ttu-id="8ad55-115">指向应用程序的隐私声明的链接。</span><span class="sxs-lookup"><span data-stu-id="8ad55-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="8ad55-116">例如，https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="8ad55-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="8ad55-117">支持</span><span class="sxs-lookup"><span data-stu-id="8ad55-117">support</span></span>|<span data-ttu-id="8ad55-118">String</span><span class="sxs-lookup"><span data-stu-id="8ad55-118">String</span></span>| <span data-ttu-id="8ad55-119">指向应用程序的支持页的链接。</span><span class="sxs-lookup"><span data-stu-id="8ad55-119">Link to the application's support page.</span></span> <span data-ttu-id="8ad55-120">例如，https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="8ad55-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="8ad55-121">termsOfService</span><span class="sxs-lookup"><span data-stu-id="8ad55-121">termsOfService</span></span>|<span data-ttu-id="8ad55-122">String</span><span class="sxs-lookup"><span data-stu-id="8ad55-122">String</span></span>| <span data-ttu-id="8ad55-123">指向应用程序的服务条款声明的链接。</span><span class="sxs-lookup"><span data-stu-id="8ad55-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="8ad55-124">例如，https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="8ad55-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8ad55-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ad55-125">JSON representation</span></span>
<span data-ttu-id="8ad55-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ad55-126">Here is a JSON representation of the resource.</span></span>

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
