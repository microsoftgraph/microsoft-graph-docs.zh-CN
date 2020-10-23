---
title: edgeSearchEngineCustom 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 85e25641fe03a4baa090a3d1fa7afe33978a9c35
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728589"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="b2e93-103">edgeSearchEngineCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2e93-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="b2e93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2e93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2e93-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2e93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2e93-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2e93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2e93-107">允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="b2e93-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="b2e93-108">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="b2e93-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2e93-109">属性</span><span class="sxs-lookup"><span data-stu-id="b2e93-109">Properties</span></span>
|<span data-ttu-id="b2e93-110">属性</span><span class="sxs-lookup"><span data-stu-id="b2e93-110">Property</span></span>|<span data-ttu-id="b2e93-111">类型</span><span class="sxs-lookup"><span data-stu-id="b2e93-111">Type</span></span>|<span data-ttu-id="b2e93-112">说明</span><span class="sxs-lookup"><span data-stu-id="b2e93-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2e93-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="b2e93-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="b2e93-114">String</span><span class="sxs-lookup"><span data-stu-id="b2e93-114">String</span></span>|<span data-ttu-id="b2e93-115">指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。</span><span class="sxs-lookup"><span data-stu-id="b2e93-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2e93-116">关系</span><span class="sxs-lookup"><span data-stu-id="b2e93-116">Relationships</span></span>
<span data-ttu-id="b2e93-117">无</span><span class="sxs-lookup"><span data-stu-id="b2e93-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2e93-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2e93-118">JSON Representation</span></span>
<span data-ttu-id="b2e93-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2e93-119">Here is a JSON representation of the resource.</span></span>
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





