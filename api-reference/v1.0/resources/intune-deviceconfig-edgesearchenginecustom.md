---
title: edgeSearchEngineCustom 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 523a2de33619886997cbcb052079bbf2937c9d48
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541225"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="22b00-103">edgeSearchEngineCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="22b00-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="22b00-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22b00-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22b00-105">允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="22b00-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="22b00-106">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="22b00-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="22b00-107">属性</span><span class="sxs-lookup"><span data-stu-id="22b00-107">Properties</span></span>
|<span data-ttu-id="22b00-108">属性</span><span class="sxs-lookup"><span data-stu-id="22b00-108">Property</span></span>|<span data-ttu-id="22b00-109">类型</span><span class="sxs-lookup"><span data-stu-id="22b00-109">Type</span></span>|<span data-ttu-id="22b00-110">说明</span><span class="sxs-lookup"><span data-stu-id="22b00-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22b00-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="22b00-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="22b00-112">String</span><span class="sxs-lookup"><span data-stu-id="22b00-112">String</span></span>|<span data-ttu-id="22b00-113">指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。</span><span class="sxs-lookup"><span data-stu-id="22b00-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22b00-114">关系</span><span class="sxs-lookup"><span data-stu-id="22b00-114">Relationships</span></span>
<span data-ttu-id="22b00-115">无</span><span class="sxs-lookup"><span data-stu-id="22b00-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22b00-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22b00-116">JSON Representation</span></span>
<span data-ttu-id="22b00-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22b00-117">Here is a JSON representation of the resource.</span></span>
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



