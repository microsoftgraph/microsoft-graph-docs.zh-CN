---
title: edgeSearchEngineCustom 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。
ms.openlocfilehash: 5312f53e43921d71e6c338ccb112a851773abc43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044534"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="ff294-103">edgeSearchEngineCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff294-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="ff294-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ff294-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff294-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ff294-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff294-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ff294-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff294-107">允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="ff294-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="ff294-108">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="ff294-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff294-109">属性</span><span class="sxs-lookup"><span data-stu-id="ff294-109">Properties</span></span>
|<span data-ttu-id="ff294-110">属性</span><span class="sxs-lookup"><span data-stu-id="ff294-110">Property</span></span>|<span data-ttu-id="ff294-111">类型</span><span class="sxs-lookup"><span data-stu-id="ff294-111">Type</span></span>|<span data-ttu-id="ff294-112">说明</span><span class="sxs-lookup"><span data-stu-id="ff294-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff294-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="ff294-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="ff294-114">String</span><span class="sxs-lookup"><span data-stu-id="ff294-114">String</span></span>|<span data-ttu-id="ff294-115">指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。</span><span class="sxs-lookup"><span data-stu-id="ff294-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff294-116">关系</span><span class="sxs-lookup"><span data-stu-id="ff294-116">Relationships</span></span>
<span data-ttu-id="ff294-117">无</span><span class="sxs-lookup"><span data-stu-id="ff294-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff294-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff294-118">JSON Representation</span></span>
<span data-ttu-id="ff294-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff294-119">Here is a JSON representation of the resource.</span></span>
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





