---
title: edgeSearchEngineCustom 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38308433f5e68d921a98e7b030540c465b33fe44
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957933"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="61bf8-103">edgeSearchEngineCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="61bf8-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="61bf8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="61bf8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61bf8-105">允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="61bf8-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="61bf8-106">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="61bf8-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="61bf8-107">属性</span><span class="sxs-lookup"><span data-stu-id="61bf8-107">Properties</span></span>
|<span data-ttu-id="61bf8-108">属性</span><span class="sxs-lookup"><span data-stu-id="61bf8-108">Property</span></span>|<span data-ttu-id="61bf8-109">类型</span><span class="sxs-lookup"><span data-stu-id="61bf8-109">Type</span></span>|<span data-ttu-id="61bf8-110">说明</span><span class="sxs-lookup"><span data-stu-id="61bf8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61bf8-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="61bf8-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="61bf8-112">String</span><span class="sxs-lookup"><span data-stu-id="61bf8-112">String</span></span>|<span data-ttu-id="61bf8-113">指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。</span><span class="sxs-lookup"><span data-stu-id="61bf8-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61bf8-114">关系</span><span class="sxs-lookup"><span data-stu-id="61bf8-114">Relationships</span></span>
<span data-ttu-id="61bf8-115">无</span><span class="sxs-lookup"><span data-stu-id="61bf8-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61bf8-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61bf8-116">JSON Representation</span></span>
<span data-ttu-id="61bf8-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61bf8-117">Here is a JSON representation of the resource.</span></span>
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



