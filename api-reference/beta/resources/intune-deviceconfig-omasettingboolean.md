---
title: omaSettingBoolean 资源类型
description: OMA 设置布尔定义。
ms.openlocfilehash: 2f2f156dba23fdba0f11667bf6d0c107e3cf74b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042841"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="f5dbd-103">omaSettingBoolean 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5dbd-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="f5dbd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f5dbd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5dbd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f5dbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5dbd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f5dbd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5dbd-107">OMA 设置布尔定义。</span><span class="sxs-lookup"><span data-stu-id="f5dbd-107">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="f5dbd-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f5dbd-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f5dbd-109">属性</span><span class="sxs-lookup"><span data-stu-id="f5dbd-109">Properties</span></span>
|<span data-ttu-id="f5dbd-110">属性</span><span class="sxs-lookup"><span data-stu-id="f5dbd-110">Property</span></span>|<span data-ttu-id="f5dbd-111">类型</span><span class="sxs-lookup"><span data-stu-id="f5dbd-111">Type</span></span>|<span data-ttu-id="f5dbd-112">说明</span><span class="sxs-lookup"><span data-stu-id="f5dbd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5dbd-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f5dbd-113">displayName</span></span>|<span data-ttu-id="f5dbd-114">String</span><span class="sxs-lookup"><span data-stu-id="f5dbd-114">String</span></span>|<span data-ttu-id="f5dbd-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="f5dbd-115">Display Name.</span></span> <span data-ttu-id="f5dbd-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f5dbd-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f5dbd-117">description</span><span class="sxs-lookup"><span data-stu-id="f5dbd-117">description</span></span>|<span data-ttu-id="f5dbd-118">String</span><span class="sxs-lookup"><span data-stu-id="f5dbd-118">String</span></span>|<span data-ttu-id="f5dbd-119">说明。</span><span class="sxs-lookup"><span data-stu-id="f5dbd-119">Description.</span></span> <span data-ttu-id="f5dbd-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f5dbd-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f5dbd-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="f5dbd-121">omaUri</span></span>|<span data-ttu-id="f5dbd-122">String</span><span class="sxs-lookup"><span data-stu-id="f5dbd-122">String</span></span>|<span data-ttu-id="f5dbd-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="f5dbd-123">OMA.</span></span> <span data-ttu-id="f5dbd-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f5dbd-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f5dbd-125">value</span><span class="sxs-lookup"><span data-stu-id="f5dbd-125">value</span></span>|<span data-ttu-id="f5dbd-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5dbd-126">Boolean</span></span>|<span data-ttu-id="f5dbd-127">值。</span><span class="sxs-lookup"><span data-stu-id="f5dbd-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5dbd-128">关系</span><span class="sxs-lookup"><span data-stu-id="f5dbd-128">Relationships</span></span>
<span data-ttu-id="f5dbd-129">无</span><span class="sxs-lookup"><span data-stu-id="f5dbd-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f5dbd-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5dbd-130">JSON Representation</span></span>
<span data-ttu-id="f5dbd-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5dbd-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```





