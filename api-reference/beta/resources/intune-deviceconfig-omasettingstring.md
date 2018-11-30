---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
ms.openlocfilehash: e0137a3d1ce7d950c107c7a63e0e5a399b3bf6d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044655"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="7e651-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e651-103">omaSettingString resource type</span></span>

> <span data-ttu-id="7e651-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7e651-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e651-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7e651-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e651-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7e651-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e651-107">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="7e651-107">OMA Settings String definition.</span></span>

<span data-ttu-id="7e651-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7e651-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e651-109">属性</span><span class="sxs-lookup"><span data-stu-id="7e651-109">Properties</span></span>
|<span data-ttu-id="7e651-110">属性</span><span class="sxs-lookup"><span data-stu-id="7e651-110">Property</span></span>|<span data-ttu-id="7e651-111">类型</span><span class="sxs-lookup"><span data-stu-id="7e651-111">Type</span></span>|<span data-ttu-id="7e651-112">说明</span><span class="sxs-lookup"><span data-stu-id="7e651-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e651-113">displayName</span><span class="sxs-lookup"><span data-stu-id="7e651-113">displayName</span></span>|<span data-ttu-id="7e651-114">String</span><span class="sxs-lookup"><span data-stu-id="7e651-114">String</span></span>|<span data-ttu-id="7e651-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="7e651-115">Display Name.</span></span> <span data-ttu-id="7e651-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7e651-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7e651-117">description</span><span class="sxs-lookup"><span data-stu-id="7e651-117">description</span></span>|<span data-ttu-id="7e651-118">String</span><span class="sxs-lookup"><span data-stu-id="7e651-118">String</span></span>|<span data-ttu-id="7e651-119">说明。</span><span class="sxs-lookup"><span data-stu-id="7e651-119">Description.</span></span> <span data-ttu-id="7e651-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7e651-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7e651-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="7e651-121">omaUri</span></span>|<span data-ttu-id="7e651-122">String</span><span class="sxs-lookup"><span data-stu-id="7e651-122">String</span></span>|<span data-ttu-id="7e651-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="7e651-123">OMA.</span></span> <span data-ttu-id="7e651-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7e651-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7e651-125">值</span><span class="sxs-lookup"><span data-stu-id="7e651-125">value</span></span>|<span data-ttu-id="7e651-126">String</span><span class="sxs-lookup"><span data-stu-id="7e651-126">String</span></span>|<span data-ttu-id="7e651-127">值。</span><span class="sxs-lookup"><span data-stu-id="7e651-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e651-128">关系</span><span class="sxs-lookup"><span data-stu-id="7e651-128">Relationships</span></span>
<span data-ttu-id="7e651-129">无</span><span class="sxs-lookup"><span data-stu-id="7e651-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7e651-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e651-130">JSON Representation</span></span>
<span data-ttu-id="7e651-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e651-131">Here is a JSON representation of the resource.</span></span>
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





