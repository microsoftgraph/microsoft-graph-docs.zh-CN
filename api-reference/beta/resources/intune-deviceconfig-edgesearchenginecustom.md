---
title: edgeSearchEngineCustom 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 69395d09c01c1b92f2ae3ee1abf26eeff09618f8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425979"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="b027e-103">edgeSearchEngineCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="b027e-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="b027e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b027e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b027e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b027e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b027e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b027e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b027e-107">允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="b027e-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="b027e-108">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="b027e-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b027e-109">属性</span><span class="sxs-lookup"><span data-stu-id="b027e-109">Properties</span></span>
|<span data-ttu-id="b027e-110">属性</span><span class="sxs-lookup"><span data-stu-id="b027e-110">Property</span></span>|<span data-ttu-id="b027e-111">类型</span><span class="sxs-lookup"><span data-stu-id="b027e-111">Type</span></span>|<span data-ttu-id="b027e-112">说明</span><span class="sxs-lookup"><span data-stu-id="b027e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b027e-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="b027e-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="b027e-114">String</span><span class="sxs-lookup"><span data-stu-id="b027e-114">String</span></span>|<span data-ttu-id="b027e-115">指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。</span><span class="sxs-lookup"><span data-stu-id="b027e-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b027e-116">关系</span><span class="sxs-lookup"><span data-stu-id="b027e-116">Relationships</span></span>
<span data-ttu-id="b027e-117">无</span><span class="sxs-lookup"><span data-stu-id="b027e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b027e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b027e-118">JSON Representation</span></span>
<span data-ttu-id="b027e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b027e-119">Here is a JSON representation of the resource.</span></span>
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




