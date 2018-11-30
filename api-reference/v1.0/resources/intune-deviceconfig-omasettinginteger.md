---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
ms.openlocfilehash: 36c22b423161d9f3c58c3085fb7b040c663d460b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011121"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="0ff43-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ff43-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="0ff43-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0ff43-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ff43-105">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="0ff43-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="0ff43-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0ff43-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ff43-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ff43-107">Properties</span></span>
|<span data-ttu-id="0ff43-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ff43-108">Property</span></span>|<span data-ttu-id="0ff43-109">类型</span><span class="sxs-lookup"><span data-stu-id="0ff43-109">Type</span></span>|<span data-ttu-id="0ff43-110">说明</span><span class="sxs-lookup"><span data-stu-id="0ff43-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ff43-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0ff43-111">displayName</span></span>|<span data-ttu-id="0ff43-112">String</span><span class="sxs-lookup"><span data-stu-id="0ff43-112">String</span></span>|<span data-ttu-id="0ff43-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="0ff43-113">Display Name.</span></span> <span data-ttu-id="0ff43-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0ff43-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0ff43-115">description</span><span class="sxs-lookup"><span data-stu-id="0ff43-115">description</span></span>|<span data-ttu-id="0ff43-116">String</span><span class="sxs-lookup"><span data-stu-id="0ff43-116">String</span></span>|<span data-ttu-id="0ff43-117">说明。</span><span class="sxs-lookup"><span data-stu-id="0ff43-117">Description.</span></span> <span data-ttu-id="0ff43-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0ff43-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0ff43-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="0ff43-119">omaUri</span></span>|<span data-ttu-id="0ff43-120">String</span><span class="sxs-lookup"><span data-stu-id="0ff43-120">String</span></span>|<span data-ttu-id="0ff43-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="0ff43-121">OMA.</span></span> <span data-ttu-id="0ff43-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0ff43-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0ff43-123">值</span><span class="sxs-lookup"><span data-stu-id="0ff43-123">value</span></span>|<span data-ttu-id="0ff43-124">Int32</span><span class="sxs-lookup"><span data-stu-id="0ff43-124">Int32</span></span>|<span data-ttu-id="0ff43-125">值。</span><span class="sxs-lookup"><span data-stu-id="0ff43-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ff43-126">关系</span><span class="sxs-lookup"><span data-stu-id="0ff43-126">Relationships</span></span>
<span data-ttu-id="0ff43-127">无</span><span class="sxs-lookup"><span data-stu-id="0ff43-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0ff43-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ff43-128">JSON Representation</span></span>
<span data-ttu-id="0ff43-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ff43-129">Here is a JSON representation of the resource.</span></span>
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



