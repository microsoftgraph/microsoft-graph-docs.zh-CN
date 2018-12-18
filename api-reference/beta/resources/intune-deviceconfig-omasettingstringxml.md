---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
author: tfitzmac
ms.openlocfilehash: 5582ca84a9d6c918ce7b8dea5a21f616804da4ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323784"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="ffc61-103">omaSettingStringXml 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffc61-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="ffc61-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ffc61-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffc61-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ffc61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffc61-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ffc61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffc61-107">OMA 设置字符串 XML 定义。</span><span class="sxs-lookup"><span data-stu-id="ffc61-107">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="ffc61-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ffc61-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ffc61-109">属性</span><span class="sxs-lookup"><span data-stu-id="ffc61-109">Properties</span></span>
|<span data-ttu-id="ffc61-110">属性</span><span class="sxs-lookup"><span data-stu-id="ffc61-110">Property</span></span>|<span data-ttu-id="ffc61-111">类型</span><span class="sxs-lookup"><span data-stu-id="ffc61-111">Type</span></span>|<span data-ttu-id="ffc61-112">说明</span><span class="sxs-lookup"><span data-stu-id="ffc61-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffc61-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ffc61-113">displayName</span></span>|<span data-ttu-id="ffc61-114">String</span><span class="sxs-lookup"><span data-stu-id="ffc61-114">String</span></span>|<span data-ttu-id="ffc61-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="ffc61-115">Display Name.</span></span> <span data-ttu-id="ffc61-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ffc61-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ffc61-117">description</span><span class="sxs-lookup"><span data-stu-id="ffc61-117">description</span></span>|<span data-ttu-id="ffc61-118">String</span><span class="sxs-lookup"><span data-stu-id="ffc61-118">String</span></span>|<span data-ttu-id="ffc61-119">说明。</span><span class="sxs-lookup"><span data-stu-id="ffc61-119">Description.</span></span> <span data-ttu-id="ffc61-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ffc61-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ffc61-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="ffc61-121">omaUri</span></span>|<span data-ttu-id="ffc61-122">String</span><span class="sxs-lookup"><span data-stu-id="ffc61-122">String</span></span>|<span data-ttu-id="ffc61-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="ffc61-123">OMA.</span></span> <span data-ttu-id="ffc61-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ffc61-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ffc61-125">fileName</span><span class="sxs-lookup"><span data-stu-id="ffc61-125">fileName</span></span>|<span data-ttu-id="ffc61-126">String</span><span class="sxs-lookup"><span data-stu-id="ffc61-126">String</span></span>|<span data-ttu-id="ffc61-127">与 Value 属性关联的文件名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="ffc61-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="ffc61-128">value</span><span class="sxs-lookup"><span data-stu-id="ffc61-128">value</span></span>|<span data-ttu-id="ffc61-129">Binary</span><span class="sxs-lookup"><span data-stu-id="ffc61-129">Binary</span></span>|<span data-ttu-id="ffc61-130">值。</span><span class="sxs-lookup"><span data-stu-id="ffc61-130">Value.</span></span> <span data-ttu-id="ffc61-131">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="ffc61-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffc61-132">关系</span><span class="sxs-lookup"><span data-stu-id="ffc61-132">Relationships</span></span>
<span data-ttu-id="ffc61-133">无</span><span class="sxs-lookup"><span data-stu-id="ffc61-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ffc61-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffc61-134">JSON Representation</span></span>
<span data-ttu-id="ffc61-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffc61-135">Here is a JSON representation of the resource.</span></span>
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





