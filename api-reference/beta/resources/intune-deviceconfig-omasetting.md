---
title: omaSetting 资源类型
description: OMA 设置定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 411e3909a71d94be2c6086e9a00616245fca062b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525983"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="1694a-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="1694a-103">omaSetting resource type</span></span>

<span data-ttu-id="1694a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1694a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1694a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1694a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1694a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1694a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1694a-107">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="1694a-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="1694a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1694a-108">Properties</span></span>
|<span data-ttu-id="1694a-109">属性</span><span class="sxs-lookup"><span data-stu-id="1694a-109">Property</span></span>|<span data-ttu-id="1694a-110">类型</span><span class="sxs-lookup"><span data-stu-id="1694a-110">Type</span></span>|<span data-ttu-id="1694a-111">说明</span><span class="sxs-lookup"><span data-stu-id="1694a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1694a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1694a-112">displayName</span></span>|<span data-ttu-id="1694a-113">字符串</span><span class="sxs-lookup"><span data-stu-id="1694a-113">String</span></span>|<span data-ttu-id="1694a-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="1694a-114">Display Name.</span></span>|
|<span data-ttu-id="1694a-115">说明</span><span class="sxs-lookup"><span data-stu-id="1694a-115">description</span></span>|<span data-ttu-id="1694a-116">String</span><span class="sxs-lookup"><span data-stu-id="1694a-116">String</span></span>|<span data-ttu-id="1694a-117">说明。</span><span class="sxs-lookup"><span data-stu-id="1694a-117">Description.</span></span>|
|<span data-ttu-id="1694a-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="1694a-118">omaUri</span></span>|<span data-ttu-id="1694a-119">String</span><span class="sxs-lookup"><span data-stu-id="1694a-119">String</span></span>|<span data-ttu-id="1694a-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="1694a-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1694a-121">关系</span><span class="sxs-lookup"><span data-stu-id="1694a-121">Relationships</span></span>
<span data-ttu-id="1694a-122">无</span><span class="sxs-lookup"><span data-stu-id="1694a-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1694a-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1694a-123">JSON Representation</span></span>
<span data-ttu-id="1694a-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1694a-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



