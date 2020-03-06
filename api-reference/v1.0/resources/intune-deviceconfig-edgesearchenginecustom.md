---
title: edgeSearchEngineCustom 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d48793eed6930b21defdb1f8f7aa921cdece2e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532540"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="0e775-103">edgeSearchEngineCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e775-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="0e775-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e775-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e775-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e775-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e775-106">允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="0e775-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="0e775-107">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="0e775-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0e775-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e775-108">Properties</span></span>
|<span data-ttu-id="0e775-109">属性</span><span class="sxs-lookup"><span data-stu-id="0e775-109">Property</span></span>|<span data-ttu-id="0e775-110">类型</span><span class="sxs-lookup"><span data-stu-id="0e775-110">Type</span></span>|<span data-ttu-id="0e775-111">说明</span><span class="sxs-lookup"><span data-stu-id="0e775-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e775-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="0e775-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="0e775-113">String</span><span class="sxs-lookup"><span data-stu-id="0e775-113">String</span></span>|<span data-ttu-id="0e775-114">指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。</span><span class="sxs-lookup"><span data-stu-id="0e775-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e775-115">关系</span><span class="sxs-lookup"><span data-stu-id="0e775-115">Relationships</span></span>
<span data-ttu-id="0e775-116">无</span><span class="sxs-lookup"><span data-stu-id="0e775-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e775-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e775-117">JSON Representation</span></span>
<span data-ttu-id="0e775-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e775-118">Here is a JSON representation of the resource.</span></span>
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




