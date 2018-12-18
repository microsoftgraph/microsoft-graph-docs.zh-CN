---
title: edgeSearchEngineCustom 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。
author: tfitzmac
ms.openlocfilehash: 1a9c1dc12226bf13764a155e804d379d20825103
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344231"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="5ad51-103">edgeSearchEngineCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ad51-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="5ad51-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5ad51-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ad51-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5ad51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ad51-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5ad51-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ad51-107">允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="5ad51-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="5ad51-108">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="5ad51-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5ad51-109">属性</span><span class="sxs-lookup"><span data-stu-id="5ad51-109">Properties</span></span>
|<span data-ttu-id="5ad51-110">属性</span><span class="sxs-lookup"><span data-stu-id="5ad51-110">Property</span></span>|<span data-ttu-id="5ad51-111">类型</span><span class="sxs-lookup"><span data-stu-id="5ad51-111">Type</span></span>|<span data-ttu-id="5ad51-112">说明</span><span class="sxs-lookup"><span data-stu-id="5ad51-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ad51-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="5ad51-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="5ad51-114">String</span><span class="sxs-lookup"><span data-stu-id="5ad51-114">String</span></span>|<span data-ttu-id="5ad51-115">指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。</span><span class="sxs-lookup"><span data-stu-id="5ad51-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ad51-116">关系</span><span class="sxs-lookup"><span data-stu-id="5ad51-116">Relationships</span></span>
<span data-ttu-id="5ad51-117">无</span><span class="sxs-lookup"><span data-stu-id="5ad51-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5ad51-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ad51-118">JSON Representation</span></span>
<span data-ttu-id="5ad51-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ad51-119">Here is a JSON representation of the resource.</span></span>
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





