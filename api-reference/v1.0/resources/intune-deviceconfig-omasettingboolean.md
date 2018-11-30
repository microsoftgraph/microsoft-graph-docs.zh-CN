---
title: omaSettingBoolean 资源类型
description: OMA 设置布尔定义。
ms.openlocfilehash: 1c0cc1d90374b7720fd9ba95e7488a09167f7842
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009011"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="897f8-103">omaSettingBoolean 资源类型</span><span class="sxs-lookup"><span data-stu-id="897f8-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="897f8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="897f8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="897f8-105">OMA 设置布尔定义。</span><span class="sxs-lookup"><span data-stu-id="897f8-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="897f8-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="897f8-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="897f8-107">属性</span><span class="sxs-lookup"><span data-stu-id="897f8-107">Properties</span></span>
|<span data-ttu-id="897f8-108">属性</span><span class="sxs-lookup"><span data-stu-id="897f8-108">Property</span></span>|<span data-ttu-id="897f8-109">类型</span><span class="sxs-lookup"><span data-stu-id="897f8-109">Type</span></span>|<span data-ttu-id="897f8-110">说明</span><span class="sxs-lookup"><span data-stu-id="897f8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="897f8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="897f8-111">displayName</span></span>|<span data-ttu-id="897f8-112">String</span><span class="sxs-lookup"><span data-stu-id="897f8-112">String</span></span>|<span data-ttu-id="897f8-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="897f8-113">Display Name.</span></span> <span data-ttu-id="897f8-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="897f8-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="897f8-115">description</span><span class="sxs-lookup"><span data-stu-id="897f8-115">description</span></span>|<span data-ttu-id="897f8-116">String</span><span class="sxs-lookup"><span data-stu-id="897f8-116">String</span></span>|<span data-ttu-id="897f8-117">说明。</span><span class="sxs-lookup"><span data-stu-id="897f8-117">Description.</span></span> <span data-ttu-id="897f8-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="897f8-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="897f8-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="897f8-119">omaUri</span></span>|<span data-ttu-id="897f8-120">String</span><span class="sxs-lookup"><span data-stu-id="897f8-120">String</span></span>|<span data-ttu-id="897f8-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="897f8-121">OMA.</span></span> <span data-ttu-id="897f8-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="897f8-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="897f8-123">value</span><span class="sxs-lookup"><span data-stu-id="897f8-123">value</span></span>|<span data-ttu-id="897f8-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="897f8-124">Boolean</span></span>|<span data-ttu-id="897f8-125">值。</span><span class="sxs-lookup"><span data-stu-id="897f8-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="897f8-126">关系</span><span class="sxs-lookup"><span data-stu-id="897f8-126">Relationships</span></span>
<span data-ttu-id="897f8-127">无</span><span class="sxs-lookup"><span data-stu-id="897f8-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="897f8-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="897f8-128">JSON Representation</span></span>
<span data-ttu-id="897f8-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="897f8-129">Here is a JSON representation of the resource.</span></span>
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



