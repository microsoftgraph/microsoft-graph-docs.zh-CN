---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: efc9a2ddd996088f88b85be55c9c7d6bfe62b86a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000786"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="4100a-103">omaSettingStringXml 资源类型</span><span class="sxs-lookup"><span data-stu-id="4100a-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="4100a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4100a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4100a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4100a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4100a-106">OMA 设置字符串 XML 定义。</span><span class="sxs-lookup"><span data-stu-id="4100a-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="4100a-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4100a-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4100a-108">属性</span><span class="sxs-lookup"><span data-stu-id="4100a-108">Properties</span></span>
|<span data-ttu-id="4100a-109">属性</span><span class="sxs-lookup"><span data-stu-id="4100a-109">Property</span></span>|<span data-ttu-id="4100a-110">类型</span><span class="sxs-lookup"><span data-stu-id="4100a-110">Type</span></span>|<span data-ttu-id="4100a-111">说明</span><span class="sxs-lookup"><span data-stu-id="4100a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4100a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4100a-112">displayName</span></span>|<span data-ttu-id="4100a-113">字符串</span><span class="sxs-lookup"><span data-stu-id="4100a-113">String</span></span>|<span data-ttu-id="4100a-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="4100a-114">Display Name.</span></span> <span data-ttu-id="4100a-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4100a-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4100a-116">说明</span><span class="sxs-lookup"><span data-stu-id="4100a-116">description</span></span>|<span data-ttu-id="4100a-117">String</span><span class="sxs-lookup"><span data-stu-id="4100a-117">String</span></span>|<span data-ttu-id="4100a-118">说明。</span><span class="sxs-lookup"><span data-stu-id="4100a-118">Description.</span></span> <span data-ttu-id="4100a-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4100a-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4100a-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="4100a-120">omaUri</span></span>|<span data-ttu-id="4100a-121">String</span><span class="sxs-lookup"><span data-stu-id="4100a-121">String</span></span>|<span data-ttu-id="4100a-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="4100a-122">OMA.</span></span> <span data-ttu-id="4100a-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4100a-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4100a-124">fileName</span><span class="sxs-lookup"><span data-stu-id="4100a-124">fileName</span></span>|<span data-ttu-id="4100a-125">String</span><span class="sxs-lookup"><span data-stu-id="4100a-125">String</span></span>|<span data-ttu-id="4100a-126">与 Value 属性关联的文件名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="4100a-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="4100a-127">value</span><span class="sxs-lookup"><span data-stu-id="4100a-127">value</span></span>|<span data-ttu-id="4100a-128">Binary</span><span class="sxs-lookup"><span data-stu-id="4100a-128">Binary</span></span>|<span data-ttu-id="4100a-129">值。</span><span class="sxs-lookup"><span data-stu-id="4100a-129">Value.</span></span> <span data-ttu-id="4100a-130">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="4100a-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4100a-131">关系</span><span class="sxs-lookup"><span data-stu-id="4100a-131">Relationships</span></span>
<span data-ttu-id="4100a-132">无</span><span class="sxs-lookup"><span data-stu-id="4100a-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4100a-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4100a-133">JSON Representation</span></span>
<span data-ttu-id="4100a-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4100a-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```





