---
title: unsupportedDeviceConfigurationDetail 资源类型
description: 为什么说实体是不受支持的说明。
author: tfitzmac
ms.openlocfilehash: 4cccf49366a803e5f964605a4dc4ba7f56707823
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344049"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="74932-103">unsupportedDeviceConfigurationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="74932-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="74932-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="74932-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74932-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="74932-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74932-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="74932-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74932-107">为什么说实体是不受支持的说明。</span><span class="sxs-lookup"><span data-stu-id="74932-107">A description of why an entity is unsupported.</span></span>
## <a name="properties"></a><span data-ttu-id="74932-108">属性</span><span class="sxs-lookup"><span data-stu-id="74932-108">Properties</span></span>
|<span data-ttu-id="74932-109">属性</span><span class="sxs-lookup"><span data-stu-id="74932-109">Property</span></span>|<span data-ttu-id="74932-110">类型</span><span class="sxs-lookup"><span data-stu-id="74932-110">Type</span></span>|<span data-ttu-id="74932-111">说明</span><span class="sxs-lookup"><span data-stu-id="74932-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74932-112">message</span><span class="sxs-lookup"><span data-stu-id="74932-112">message</span></span>|<span data-ttu-id="74932-113">字符串</span><span class="sxs-lookup"><span data-stu-id="74932-113">String</span></span>|<span data-ttu-id="74932-114">解释 entity 为什么不受支持的一条消息。</span><span class="sxs-lookup"><span data-stu-id="74932-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="74932-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="74932-115">propertyName</span></span>|<span data-ttu-id="74932-116">字符串</span><span class="sxs-lookup"><span data-stu-id="74932-116">String</span></span>|<span data-ttu-id="74932-117">如果邮件与原始实体，则该属性的名称中的特定属性。</span><span class="sxs-lookup"><span data-stu-id="74932-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74932-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="74932-118">Relationships</span></span>
<span data-ttu-id="74932-119">无</span><span class="sxs-lookup"><span data-stu-id="74932-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="74932-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74932-120">JSON Representation</span></span>
<span data-ttu-id="74932-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74932-121">Here is a JSON representation of the resource.</span></span>
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





