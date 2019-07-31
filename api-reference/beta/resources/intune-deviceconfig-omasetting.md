---
title: omaSetting 资源类型
description: OMA 设置定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58de40a93fe85c1eb58b558cf44214358070901d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969973"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="95048-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="95048-103">omaSetting resource type</span></span>

> <span data-ttu-id="95048-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95048-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95048-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95048-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95048-106">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="95048-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="95048-107">属性</span><span class="sxs-lookup"><span data-stu-id="95048-107">Properties</span></span>
|<span data-ttu-id="95048-108">属性</span><span class="sxs-lookup"><span data-stu-id="95048-108">Property</span></span>|<span data-ttu-id="95048-109">类型</span><span class="sxs-lookup"><span data-stu-id="95048-109">Type</span></span>|<span data-ttu-id="95048-110">说明</span><span class="sxs-lookup"><span data-stu-id="95048-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95048-111">displayName</span><span class="sxs-lookup"><span data-stu-id="95048-111">displayName</span></span>|<span data-ttu-id="95048-112">字符串</span><span class="sxs-lookup"><span data-stu-id="95048-112">String</span></span>|<span data-ttu-id="95048-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="95048-113">Display Name.</span></span>|
|<span data-ttu-id="95048-114">说明</span><span class="sxs-lookup"><span data-stu-id="95048-114">description</span></span>|<span data-ttu-id="95048-115">String</span><span class="sxs-lookup"><span data-stu-id="95048-115">String</span></span>|<span data-ttu-id="95048-116">说明。</span><span class="sxs-lookup"><span data-stu-id="95048-116">Description.</span></span>|
|<span data-ttu-id="95048-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="95048-117">omaUri</span></span>|<span data-ttu-id="95048-118">String</span><span class="sxs-lookup"><span data-stu-id="95048-118">String</span></span>|<span data-ttu-id="95048-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="95048-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95048-120">关系</span><span class="sxs-lookup"><span data-stu-id="95048-120">Relationships</span></span>
<span data-ttu-id="95048-121">无</span><span class="sxs-lookup"><span data-stu-id="95048-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95048-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95048-122">JSON Representation</span></span>
<span data-ttu-id="95048-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95048-123">Here is a JSON representation of the resource.</span></span>
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





