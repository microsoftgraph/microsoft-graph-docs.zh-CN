---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 998b62b639bb155e320d8293452052d8eebe41ca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952515"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="06419-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="06419-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="06419-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="06419-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06419-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="06419-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06419-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="06419-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06419-107">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="06419-107">OMA Settings Integer definition.</span></span>

<span data-ttu-id="06419-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="06419-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="06419-109">属性</span><span class="sxs-lookup"><span data-stu-id="06419-109">Properties</span></span>
|<span data-ttu-id="06419-110">属性</span><span class="sxs-lookup"><span data-stu-id="06419-110">Property</span></span>|<span data-ttu-id="06419-111">类型</span><span class="sxs-lookup"><span data-stu-id="06419-111">Type</span></span>|<span data-ttu-id="06419-112">说明</span><span class="sxs-lookup"><span data-stu-id="06419-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06419-113">displayName</span><span class="sxs-lookup"><span data-stu-id="06419-113">displayName</span></span>|<span data-ttu-id="06419-114">String</span><span class="sxs-lookup"><span data-stu-id="06419-114">String</span></span>|<span data-ttu-id="06419-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="06419-115">Display Name.</span></span> <span data-ttu-id="06419-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="06419-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="06419-117">description</span><span class="sxs-lookup"><span data-stu-id="06419-117">description</span></span>|<span data-ttu-id="06419-118">String</span><span class="sxs-lookup"><span data-stu-id="06419-118">String</span></span>|<span data-ttu-id="06419-119">说明。</span><span class="sxs-lookup"><span data-stu-id="06419-119">Description.</span></span> <span data-ttu-id="06419-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="06419-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="06419-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="06419-121">omaUri</span></span>|<span data-ttu-id="06419-122">String</span><span class="sxs-lookup"><span data-stu-id="06419-122">String</span></span>|<span data-ttu-id="06419-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="06419-123">OMA.</span></span> <span data-ttu-id="06419-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="06419-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="06419-125">值</span><span class="sxs-lookup"><span data-stu-id="06419-125">value</span></span>|<span data-ttu-id="06419-126">Int32</span><span class="sxs-lookup"><span data-stu-id="06419-126">Int32</span></span>|<span data-ttu-id="06419-127">值。</span><span class="sxs-lookup"><span data-stu-id="06419-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06419-128">关系</span><span class="sxs-lookup"><span data-stu-id="06419-128">Relationships</span></span>
<span data-ttu-id="06419-129">无</span><span class="sxs-lookup"><span data-stu-id="06419-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06419-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06419-130">JSON Representation</span></span>
<span data-ttu-id="06419-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06419-131">Here is a JSON representation of the resource.</span></span>
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





