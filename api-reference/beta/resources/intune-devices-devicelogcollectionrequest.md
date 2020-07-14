---
title: deviceLogCollectionRequest 资源类型
description: Windows 日志集合请求实体。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a7095a667ccbc3fb534a632665ef9694b89e380
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124184"
---
# <a name="devicelogcollectionrequest-resource-type"></a><span data-ttu-id="7f5bf-103">deviceLogCollectionRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f5bf-103">deviceLogCollectionRequest resource type</span></span>

<span data-ttu-id="7f5bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f5bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f5bf-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f5bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f5bf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f5bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f5bf-107">Windows 日志集合请求实体。</span><span class="sxs-lookup"><span data-stu-id="7f5bf-107">Windows Log Collection request entity.</span></span>

## <a name="properties"></a><span data-ttu-id="7f5bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f5bf-108">Properties</span></span>
|<span data-ttu-id="7f5bf-109">属性</span><span class="sxs-lookup"><span data-stu-id="7f5bf-109">Property</span></span>|<span data-ttu-id="7f5bf-110">类型</span><span class="sxs-lookup"><span data-stu-id="7f5bf-110">Type</span></span>|<span data-ttu-id="7f5bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="7f5bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f5bf-112">id</span><span class="sxs-lookup"><span data-stu-id="7f5bf-112">id</span></span>|<span data-ttu-id="7f5bf-113">String</span><span class="sxs-lookup"><span data-stu-id="7f5bf-113">String</span></span>|<span data-ttu-id="7f5bf-114">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="7f5bf-114">The unique identifier</span></span>|
|<span data-ttu-id="7f5bf-115">templateType</span><span class="sxs-lookup"><span data-stu-id="7f5bf-115">templateType</span></span>|[<span data-ttu-id="7f5bf-116">deviceLogCollectionTemplateType</span><span class="sxs-lookup"><span data-stu-id="7f5bf-116">deviceLogCollectionTemplateType</span></span>](../resources/intune-devices-devicelogcollectiontemplatetype.md)|<span data-ttu-id="7f5bf-117">与集合请求一起发送的模板类型。</span><span class="sxs-lookup"><span data-stu-id="7f5bf-117">The template type that is sent with the collection request.</span></span> <span data-ttu-id="7f5bf-118">可能的值是： `predefined` 。</span><span class="sxs-lookup"><span data-stu-id="7f5bf-118">Possible values are: `predefined`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f5bf-119">关系</span><span class="sxs-lookup"><span data-stu-id="7f5bf-119">Relationships</span></span>
<span data-ttu-id="7f5bf-120">无</span><span class="sxs-lookup"><span data-stu-id="7f5bf-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f5bf-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f5bf-121">JSON Representation</span></span>
<span data-ttu-id="7f5bf-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f5bf-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionRequest",
  "id": "String (identifier)",
  "templateType": "String"
}
```



