---
title: omaSetting 资源类型
description: OMA 设置定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fab80ad06fb5654578f29b92e3b0f3aa9c09abdb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143846"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="cda73-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="cda73-103">omaSetting resource type</span></span>

> <span data-ttu-id="cda73-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cda73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cda73-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cda73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cda73-106">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="cda73-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="cda73-107">属性</span><span class="sxs-lookup"><span data-stu-id="cda73-107">Properties</span></span>
|<span data-ttu-id="cda73-108">属性</span><span class="sxs-lookup"><span data-stu-id="cda73-108">Property</span></span>|<span data-ttu-id="cda73-109">类型</span><span class="sxs-lookup"><span data-stu-id="cda73-109">Type</span></span>|<span data-ttu-id="cda73-110">说明</span><span class="sxs-lookup"><span data-stu-id="cda73-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cda73-111">displayName</span><span class="sxs-lookup"><span data-stu-id="cda73-111">displayName</span></span>|<span data-ttu-id="cda73-112">字符串</span><span class="sxs-lookup"><span data-stu-id="cda73-112">String</span></span>|<span data-ttu-id="cda73-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="cda73-113">Display Name.</span></span>|
|<span data-ttu-id="cda73-114">description</span><span class="sxs-lookup"><span data-stu-id="cda73-114">description</span></span>|<span data-ttu-id="cda73-115">字符串</span><span class="sxs-lookup"><span data-stu-id="cda73-115">String</span></span>|<span data-ttu-id="cda73-116">说明。</span><span class="sxs-lookup"><span data-stu-id="cda73-116">Description.</span></span>|
|<span data-ttu-id="cda73-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="cda73-117">omaUri</span></span>|<span data-ttu-id="cda73-118">String</span><span class="sxs-lookup"><span data-stu-id="cda73-118">String</span></span>|<span data-ttu-id="cda73-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="cda73-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cda73-120">关系</span><span class="sxs-lookup"><span data-stu-id="cda73-120">Relationships</span></span>
<span data-ttu-id="cda73-121">无</span><span class="sxs-lookup"><span data-stu-id="cda73-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cda73-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cda73-122">JSON Representation</span></span>
<span data-ttu-id="cda73-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cda73-123">Here is a JSON representation of the resource.</span></span>
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




