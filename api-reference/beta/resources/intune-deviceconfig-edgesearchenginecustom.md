---
title: edgeSearchEngineCustom 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da4186e82eb33934d1b4b4fe191b0ee035218d92
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386076"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="c499e-103">edgeSearchEngineCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="c499e-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="c499e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c499e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c499e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c499e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c499e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c499e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c499e-107">允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="c499e-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="c499e-108">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="c499e-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c499e-109">属性</span><span class="sxs-lookup"><span data-stu-id="c499e-109">Properties</span></span>
|<span data-ttu-id="c499e-110">属性</span><span class="sxs-lookup"><span data-stu-id="c499e-110">Property</span></span>|<span data-ttu-id="c499e-111">类型</span><span class="sxs-lookup"><span data-stu-id="c499e-111">Type</span></span>|<span data-ttu-id="c499e-112">说明</span><span class="sxs-lookup"><span data-stu-id="c499e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c499e-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="c499e-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="c499e-114">String</span><span class="sxs-lookup"><span data-stu-id="c499e-114">String</span></span>|<span data-ttu-id="c499e-115">指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。</span><span class="sxs-lookup"><span data-stu-id="c499e-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c499e-116">关系</span><span class="sxs-lookup"><span data-stu-id="c499e-116">Relationships</span></span>
<span data-ttu-id="c499e-117">无</span><span class="sxs-lookup"><span data-stu-id="c499e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c499e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c499e-118">JSON Representation</span></span>
<span data-ttu-id="c499e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c499e-119">Here is a JSON representation of the resource.</span></span>
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



