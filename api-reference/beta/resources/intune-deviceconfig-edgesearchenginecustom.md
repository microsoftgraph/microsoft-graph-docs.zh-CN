---
title: edgeSearchEngineCustom 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 34e31bb35426f7aab1b2a8e824e50933e5892b5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001416"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="7700c-103">edgeSearchEngineCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="7700c-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="7700c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7700c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7700c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7700c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7700c-106">允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="7700c-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="7700c-107">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="7700c-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7700c-108">属性</span><span class="sxs-lookup"><span data-stu-id="7700c-108">Properties</span></span>
|<span data-ttu-id="7700c-109">属性</span><span class="sxs-lookup"><span data-stu-id="7700c-109">Property</span></span>|<span data-ttu-id="7700c-110">类型</span><span class="sxs-lookup"><span data-stu-id="7700c-110">Type</span></span>|<span data-ttu-id="7700c-111">说明</span><span class="sxs-lookup"><span data-stu-id="7700c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7700c-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="7700c-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="7700c-113">String</span><span class="sxs-lookup"><span data-stu-id="7700c-113">String</span></span>|<span data-ttu-id="7700c-114">指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。</span><span class="sxs-lookup"><span data-stu-id="7700c-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7700c-115">关系</span><span class="sxs-lookup"><span data-stu-id="7700c-115">Relationships</span></span>
<span data-ttu-id="7700c-116">无</span><span class="sxs-lookup"><span data-stu-id="7700c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7700c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7700c-117">JSON Representation</span></span>
<span data-ttu-id="7700c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7700c-118">Here is a JSON representation of the resource.</span></span>
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





