---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
ms.openlocfilehash: b4ea11c22acb2a4119c2de1934f1ae66c2310658
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008336"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="0e04b-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e04b-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="0e04b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0e04b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e04b-105">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="0e04b-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="0e04b-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e04b-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0e04b-107">属性</span><span class="sxs-lookup"><span data-stu-id="0e04b-107">Properties</span></span>
|<span data-ttu-id="0e04b-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e04b-108">Property</span></span>|<span data-ttu-id="0e04b-109">类型</span><span class="sxs-lookup"><span data-stu-id="0e04b-109">Type</span></span>|<span data-ttu-id="0e04b-110">说明</span><span class="sxs-lookup"><span data-stu-id="0e04b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e04b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0e04b-111">displayName</span></span>|<span data-ttu-id="0e04b-112">String</span><span class="sxs-lookup"><span data-stu-id="0e04b-112">String</span></span>|<span data-ttu-id="0e04b-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="0e04b-113">Display Name.</span></span> <span data-ttu-id="0e04b-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e04b-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0e04b-115">description</span><span class="sxs-lookup"><span data-stu-id="0e04b-115">description</span></span>|<span data-ttu-id="0e04b-116">String</span><span class="sxs-lookup"><span data-stu-id="0e04b-116">String</span></span>|<span data-ttu-id="0e04b-117">说明。</span><span class="sxs-lookup"><span data-stu-id="0e04b-117">Description.</span></span> <span data-ttu-id="0e04b-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e04b-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0e04b-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="0e04b-119">omaUri</span></span>|<span data-ttu-id="0e04b-120">String</span><span class="sxs-lookup"><span data-stu-id="0e04b-120">String</span></span>|<span data-ttu-id="0e04b-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="0e04b-121">OMA.</span></span> <span data-ttu-id="0e04b-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e04b-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0e04b-123">value</span><span class="sxs-lookup"><span data-stu-id="0e04b-123">value</span></span>|<span data-ttu-id="0e04b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e04b-124">DateTimeOffset</span></span>|<span data-ttu-id="0e04b-125">值。</span><span class="sxs-lookup"><span data-stu-id="0e04b-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e04b-126">关系</span><span class="sxs-lookup"><span data-stu-id="0e04b-126">Relationships</span></span>
<span data-ttu-id="0e04b-127">无</span><span class="sxs-lookup"><span data-stu-id="0e04b-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e04b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e04b-128">JSON Representation</span></span>
<span data-ttu-id="0e04b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e04b-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



