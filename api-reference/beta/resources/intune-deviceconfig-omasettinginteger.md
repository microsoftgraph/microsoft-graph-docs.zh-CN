---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 800c36cf769def2f040376c8c580f361cd52cde0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397860"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="29578-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="29578-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="29578-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="29578-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="29578-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="29578-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29578-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29578-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29578-107">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="29578-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="29578-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="29578-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="29578-109">属性</span><span class="sxs-lookup"><span data-stu-id="29578-109">Properties</span></span>
|<span data-ttu-id="29578-110">属性</span><span class="sxs-lookup"><span data-stu-id="29578-110">Property</span></span>|<span data-ttu-id="29578-111">类型</span><span class="sxs-lookup"><span data-stu-id="29578-111">Type</span></span>|<span data-ttu-id="29578-112">说明</span><span class="sxs-lookup"><span data-stu-id="29578-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29578-113">displayName</span><span class="sxs-lookup"><span data-stu-id="29578-113">displayName</span></span>|<span data-ttu-id="29578-114">String</span><span class="sxs-lookup"><span data-stu-id="29578-114">String</span></span>|<span data-ttu-id="29578-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="29578-115">Display Name.</span></span> <span data-ttu-id="29578-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="29578-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="29578-117">description</span><span class="sxs-lookup"><span data-stu-id="29578-117">description</span></span>|<span data-ttu-id="29578-118">String</span><span class="sxs-lookup"><span data-stu-id="29578-118">String</span></span>|<span data-ttu-id="29578-119">说明。</span><span class="sxs-lookup"><span data-stu-id="29578-119">Description.</span></span> <span data-ttu-id="29578-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="29578-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="29578-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="29578-121">omaUri</span></span>|<span data-ttu-id="29578-122">String</span><span class="sxs-lookup"><span data-stu-id="29578-122">String</span></span>|<span data-ttu-id="29578-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="29578-123">OMA.</span></span> <span data-ttu-id="29578-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="29578-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="29578-125">值</span><span class="sxs-lookup"><span data-stu-id="29578-125">value</span></span>|<span data-ttu-id="29578-126">Int32</span><span class="sxs-lookup"><span data-stu-id="29578-126">Int32</span></span>|<span data-ttu-id="29578-127">值。</span><span class="sxs-lookup"><span data-stu-id="29578-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29578-128">关系</span><span class="sxs-lookup"><span data-stu-id="29578-128">Relationships</span></span>
<span data-ttu-id="29578-129">无</span><span class="sxs-lookup"><span data-stu-id="29578-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29578-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29578-130">JSON Representation</span></span>
<span data-ttu-id="29578-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29578-131">Here is a JSON representation of the resource.</span></span>
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




