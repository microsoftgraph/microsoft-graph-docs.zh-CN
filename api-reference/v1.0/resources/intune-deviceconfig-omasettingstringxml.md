---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e34dc1ebdfff2692d35d258492bc58cb26282198
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911481"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="7735c-103">omaSettingStringXml 资源类型</span><span class="sxs-lookup"><span data-stu-id="7735c-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="7735c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7735c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7735c-105">OMA 设置字符串 XML 定义。</span><span class="sxs-lookup"><span data-stu-id="7735c-105">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="7735c-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7735c-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7735c-107">属性</span><span class="sxs-lookup"><span data-stu-id="7735c-107">Properties</span></span>
|<span data-ttu-id="7735c-108">属性</span><span class="sxs-lookup"><span data-stu-id="7735c-108">Property</span></span>|<span data-ttu-id="7735c-109">类型</span><span class="sxs-lookup"><span data-stu-id="7735c-109">Type</span></span>|<span data-ttu-id="7735c-110">说明</span><span class="sxs-lookup"><span data-stu-id="7735c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7735c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7735c-111">displayName</span></span>|<span data-ttu-id="7735c-112">String</span><span class="sxs-lookup"><span data-stu-id="7735c-112">String</span></span>|<span data-ttu-id="7735c-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="7735c-113">Display Name.</span></span> <span data-ttu-id="7735c-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7735c-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7735c-115">description</span><span class="sxs-lookup"><span data-stu-id="7735c-115">description</span></span>|<span data-ttu-id="7735c-116">String</span><span class="sxs-lookup"><span data-stu-id="7735c-116">String</span></span>|<span data-ttu-id="7735c-117">说明。</span><span class="sxs-lookup"><span data-stu-id="7735c-117">Description.</span></span> <span data-ttu-id="7735c-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7735c-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7735c-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="7735c-119">omaUri</span></span>|<span data-ttu-id="7735c-120">String</span><span class="sxs-lookup"><span data-stu-id="7735c-120">String</span></span>|<span data-ttu-id="7735c-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="7735c-121">OMA.</span></span> <span data-ttu-id="7735c-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7735c-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7735c-123">fileName</span><span class="sxs-lookup"><span data-stu-id="7735c-123">fileName</span></span>|<span data-ttu-id="7735c-124">String</span><span class="sxs-lookup"><span data-stu-id="7735c-124">String</span></span>|<span data-ttu-id="7735c-125">与 Value 属性关联的文件名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="7735c-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="7735c-126">value</span><span class="sxs-lookup"><span data-stu-id="7735c-126">value</span></span>|<span data-ttu-id="7735c-127">Binary</span><span class="sxs-lookup"><span data-stu-id="7735c-127">Binary</span></span>|<span data-ttu-id="7735c-128">值。</span><span class="sxs-lookup"><span data-stu-id="7735c-128">Value.</span></span> <span data-ttu-id="7735c-129">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="7735c-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7735c-130">关系</span><span class="sxs-lookup"><span data-stu-id="7735c-130">Relationships</span></span>
<span data-ttu-id="7735c-131">无</span><span class="sxs-lookup"><span data-stu-id="7735c-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7735c-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7735c-132">JSON Representation</span></span>
<span data-ttu-id="7735c-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7735c-133">Here is a JSON representation of the resource.</span></span>
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



