---
title: edgeSearchEngineCustom 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1f97de9b4665769ea4e9731045603664673f64f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165728"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="9734f-103">edgeSearchEngineCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="9734f-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="9734f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9734f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9734f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9734f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9734f-106">允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="9734f-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="9734f-107">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="9734f-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9734f-108">属性</span><span class="sxs-lookup"><span data-stu-id="9734f-108">Properties</span></span>
|<span data-ttu-id="9734f-109">属性</span><span class="sxs-lookup"><span data-stu-id="9734f-109">Property</span></span>|<span data-ttu-id="9734f-110">类型</span><span class="sxs-lookup"><span data-stu-id="9734f-110">Type</span></span>|<span data-ttu-id="9734f-111">说明</span><span class="sxs-lookup"><span data-stu-id="9734f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9734f-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="9734f-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="9734f-113">String</span><span class="sxs-lookup"><span data-stu-id="9734f-113">String</span></span>|<span data-ttu-id="9734f-114">指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。</span><span class="sxs-lookup"><span data-stu-id="9734f-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9734f-115">关系</span><span class="sxs-lookup"><span data-stu-id="9734f-115">Relationships</span></span>
<span data-ttu-id="9734f-116">无</span><span class="sxs-lookup"><span data-stu-id="9734f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9734f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9734f-117">JSON Representation</span></span>
<span data-ttu-id="9734f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9734f-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```




