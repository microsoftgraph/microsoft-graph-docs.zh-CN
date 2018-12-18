---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: tfitzmac
ms.openlocfilehash: a62f6dee2bf0f5a9ca96488625a84ceef5f7c785
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311198"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="b9b5e-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9b5e-103">omaSettingString resource type</span></span>

> <span data-ttu-id="b9b5e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b9b5e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9b5e-105">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="b9b5e-105">OMA Settings String definition.</span></span>

<span data-ttu-id="b9b5e-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b9b5e-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b9b5e-107">属性</span><span class="sxs-lookup"><span data-stu-id="b9b5e-107">Properties</span></span>
|<span data-ttu-id="b9b5e-108">属性</span><span class="sxs-lookup"><span data-stu-id="b9b5e-108">Property</span></span>|<span data-ttu-id="b9b5e-109">类型</span><span class="sxs-lookup"><span data-stu-id="b9b5e-109">Type</span></span>|<span data-ttu-id="b9b5e-110">说明</span><span class="sxs-lookup"><span data-stu-id="b9b5e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9b5e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b9b5e-111">displayName</span></span>|<span data-ttu-id="b9b5e-112">String</span><span class="sxs-lookup"><span data-stu-id="b9b5e-112">String</span></span>|<span data-ttu-id="b9b5e-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="b9b5e-113">Display Name.</span></span> <span data-ttu-id="b9b5e-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b9b5e-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b9b5e-115">description</span><span class="sxs-lookup"><span data-stu-id="b9b5e-115">description</span></span>|<span data-ttu-id="b9b5e-116">String</span><span class="sxs-lookup"><span data-stu-id="b9b5e-116">String</span></span>|<span data-ttu-id="b9b5e-117">说明。</span><span class="sxs-lookup"><span data-stu-id="b9b5e-117">Description.</span></span> <span data-ttu-id="b9b5e-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b9b5e-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b9b5e-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="b9b5e-119">omaUri</span></span>|<span data-ttu-id="b9b5e-120">String</span><span class="sxs-lookup"><span data-stu-id="b9b5e-120">String</span></span>|<span data-ttu-id="b9b5e-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="b9b5e-121">OMA.</span></span> <span data-ttu-id="b9b5e-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b9b5e-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b9b5e-123">值</span><span class="sxs-lookup"><span data-stu-id="b9b5e-123">value</span></span>|<span data-ttu-id="b9b5e-124">String</span><span class="sxs-lookup"><span data-stu-id="b9b5e-124">String</span></span>|<span data-ttu-id="b9b5e-125">值。</span><span class="sxs-lookup"><span data-stu-id="b9b5e-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9b5e-126">关系</span><span class="sxs-lookup"><span data-stu-id="b9b5e-126">Relationships</span></span>
<span data-ttu-id="b9b5e-127">无</span><span class="sxs-lookup"><span data-stu-id="b9b5e-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b9b5e-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9b5e-128">JSON Representation</span></span>
<span data-ttu-id="b9b5e-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9b5e-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



