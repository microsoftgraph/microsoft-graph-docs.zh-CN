---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: tfitzmac
ms.openlocfilehash: 27d38d1e1fe035ef95203ca1e636dedf7a05f103
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363604"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="39891-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="39891-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="39891-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="39891-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39891-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="39891-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39891-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="39891-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39891-107">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="39891-107">OMA Settings Integer definition.</span></span>

<span data-ttu-id="39891-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="39891-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="39891-109">属性</span><span class="sxs-lookup"><span data-stu-id="39891-109">Properties</span></span>
|<span data-ttu-id="39891-110">属性</span><span class="sxs-lookup"><span data-stu-id="39891-110">Property</span></span>|<span data-ttu-id="39891-111">类型</span><span class="sxs-lookup"><span data-stu-id="39891-111">Type</span></span>|<span data-ttu-id="39891-112">说明</span><span class="sxs-lookup"><span data-stu-id="39891-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39891-113">displayName</span><span class="sxs-lookup"><span data-stu-id="39891-113">displayName</span></span>|<span data-ttu-id="39891-114">String</span><span class="sxs-lookup"><span data-stu-id="39891-114">String</span></span>|<span data-ttu-id="39891-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="39891-115">Display Name.</span></span> <span data-ttu-id="39891-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="39891-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="39891-117">description</span><span class="sxs-lookup"><span data-stu-id="39891-117">description</span></span>|<span data-ttu-id="39891-118">String</span><span class="sxs-lookup"><span data-stu-id="39891-118">String</span></span>|<span data-ttu-id="39891-119">说明。</span><span class="sxs-lookup"><span data-stu-id="39891-119">Description.</span></span> <span data-ttu-id="39891-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="39891-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="39891-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="39891-121">omaUri</span></span>|<span data-ttu-id="39891-122">String</span><span class="sxs-lookup"><span data-stu-id="39891-122">String</span></span>|<span data-ttu-id="39891-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="39891-123">OMA.</span></span> <span data-ttu-id="39891-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="39891-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="39891-125">值</span><span class="sxs-lookup"><span data-stu-id="39891-125">value</span></span>|<span data-ttu-id="39891-126">Int32</span><span class="sxs-lookup"><span data-stu-id="39891-126">Int32</span></span>|<span data-ttu-id="39891-127">值。</span><span class="sxs-lookup"><span data-stu-id="39891-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39891-128">关系</span><span class="sxs-lookup"><span data-stu-id="39891-128">Relationships</span></span>
<span data-ttu-id="39891-129">无</span><span class="sxs-lookup"><span data-stu-id="39891-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39891-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39891-130">JSON Representation</span></span>
<span data-ttu-id="39891-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39891-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```





