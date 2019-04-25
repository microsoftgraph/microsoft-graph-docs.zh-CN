---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54eec27cf91bb1da7790ae1432452ac026bf1683
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542121"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="a7677-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7677-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="a7677-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a7677-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7677-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7677-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7677-106">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="a7677-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="a7677-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a7677-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a7677-108">属性</span><span class="sxs-lookup"><span data-stu-id="a7677-108">Properties</span></span>
|<span data-ttu-id="a7677-109">属性</span><span class="sxs-lookup"><span data-stu-id="a7677-109">Property</span></span>|<span data-ttu-id="a7677-110">类型</span><span class="sxs-lookup"><span data-stu-id="a7677-110">Type</span></span>|<span data-ttu-id="a7677-111">说明</span><span class="sxs-lookup"><span data-stu-id="a7677-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7677-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a7677-112">displayName</span></span>|<span data-ttu-id="a7677-113">字符串</span><span class="sxs-lookup"><span data-stu-id="a7677-113">String</span></span>|<span data-ttu-id="a7677-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="a7677-114">Display Name.</span></span> <span data-ttu-id="a7677-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a7677-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a7677-116">description</span><span class="sxs-lookup"><span data-stu-id="a7677-116">description</span></span>|<span data-ttu-id="a7677-117">String</span><span class="sxs-lookup"><span data-stu-id="a7677-117">String</span></span>|<span data-ttu-id="a7677-118">说明。</span><span class="sxs-lookup"><span data-stu-id="a7677-118">Description.</span></span> <span data-ttu-id="a7677-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a7677-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a7677-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="a7677-120">omaUri</span></span>|<span data-ttu-id="a7677-121">String</span><span class="sxs-lookup"><span data-stu-id="a7677-121">String</span></span>|<span data-ttu-id="a7677-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="a7677-122">OMA.</span></span> <span data-ttu-id="a7677-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a7677-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a7677-124">值</span><span class="sxs-lookup"><span data-stu-id="a7677-124">value</span></span>|<span data-ttu-id="a7677-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a7677-125">Int32</span></span>|<span data-ttu-id="a7677-126">值。</span><span class="sxs-lookup"><span data-stu-id="a7677-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7677-127">关系</span><span class="sxs-lookup"><span data-stu-id="a7677-127">Relationships</span></span>
<span data-ttu-id="a7677-128">无</span><span class="sxs-lookup"><span data-stu-id="a7677-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7677-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7677-129">JSON Representation</span></span>
<span data-ttu-id="a7677-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7677-130">Here is a JSON representation of the resource.</span></span>
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





