---
title: unsupportedDeviceConfigurationDetail 资源类型
description: 为什么说实体是不受支持的说明。
ms.openlocfilehash: d64d6aedf5da0f3cd79e2582d84fa4f19ea7ccfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043052"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="ba0f3-103">unsupportedDeviceConfigurationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba0f3-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="ba0f3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ba0f3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba0f3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ba0f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba0f3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ba0f3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba0f3-107">为什么说实体是不受支持的说明。</span><span class="sxs-lookup"><span data-stu-id="ba0f3-107">A description of why an entity is unsupported.</span></span>
## <a name="properties"></a><span data-ttu-id="ba0f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba0f3-108">Properties</span></span>
|<span data-ttu-id="ba0f3-109">属性</span><span class="sxs-lookup"><span data-stu-id="ba0f3-109">Property</span></span>|<span data-ttu-id="ba0f3-110">类型</span><span class="sxs-lookup"><span data-stu-id="ba0f3-110">Type</span></span>|<span data-ttu-id="ba0f3-111">说明</span><span class="sxs-lookup"><span data-stu-id="ba0f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba0f3-112">message</span><span class="sxs-lookup"><span data-stu-id="ba0f3-112">message</span></span>|<span data-ttu-id="ba0f3-113">字符串</span><span class="sxs-lookup"><span data-stu-id="ba0f3-113">String</span></span>|<span data-ttu-id="ba0f3-114">解释 entity 为什么不受支持的一条消息。</span><span class="sxs-lookup"><span data-stu-id="ba0f3-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="ba0f3-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="ba0f3-115">propertyName</span></span>|<span data-ttu-id="ba0f3-116">字符串</span><span class="sxs-lookup"><span data-stu-id="ba0f3-116">String</span></span>|<span data-ttu-id="ba0f3-117">如果邮件与原始实体，则该属性的名称中的特定属性。</span><span class="sxs-lookup"><span data-stu-id="ba0f3-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba0f3-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="ba0f3-118">Relationships</span></span>
<span data-ttu-id="ba0f3-119">无</span><span class="sxs-lookup"><span data-stu-id="ba0f3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ba0f3-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba0f3-120">JSON Representation</span></span>
<span data-ttu-id="ba0f3-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba0f3-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```





