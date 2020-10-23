---
title: deviceLogCollectionRequest 资源类型
description: Windows 日志集合请求实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e0be1fabe16e51c9ca9840f2417bc1d70d67b39
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694968"
---
# <a name="devicelogcollectionrequest-resource-type"></a><span data-ttu-id="de9d1-103">deviceLogCollectionRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="de9d1-103">deviceLogCollectionRequest resource type</span></span>

<span data-ttu-id="de9d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de9d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de9d1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="de9d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de9d1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de9d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de9d1-107">Windows 日志集合请求实体。</span><span class="sxs-lookup"><span data-stu-id="de9d1-107">Windows Log Collection request entity.</span></span>

## <a name="properties"></a><span data-ttu-id="de9d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="de9d1-108">Properties</span></span>
|<span data-ttu-id="de9d1-109">属性</span><span class="sxs-lookup"><span data-stu-id="de9d1-109">Property</span></span>|<span data-ttu-id="de9d1-110">类型</span><span class="sxs-lookup"><span data-stu-id="de9d1-110">Type</span></span>|<span data-ttu-id="de9d1-111">说明</span><span class="sxs-lookup"><span data-stu-id="de9d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de9d1-112">id</span><span class="sxs-lookup"><span data-stu-id="de9d1-112">id</span></span>|<span data-ttu-id="de9d1-113">String</span><span class="sxs-lookup"><span data-stu-id="de9d1-113">String</span></span>|<span data-ttu-id="de9d1-114">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="de9d1-114">The unique identifier</span></span>|
|<span data-ttu-id="de9d1-115">templateType</span><span class="sxs-lookup"><span data-stu-id="de9d1-115">templateType</span></span>|[<span data-ttu-id="de9d1-116">deviceLogCollectionTemplateType</span><span class="sxs-lookup"><span data-stu-id="de9d1-116">deviceLogCollectionTemplateType</span></span>](../resources/intune-devices-devicelogcollectiontemplatetype.md)|<span data-ttu-id="de9d1-117">与集合请求一起发送的模板类型。</span><span class="sxs-lookup"><span data-stu-id="de9d1-117">The template type that is sent with the collection request.</span></span> <span data-ttu-id="de9d1-118">可能的值是： `predefined` 。</span><span class="sxs-lookup"><span data-stu-id="de9d1-118">Possible values are: `predefined`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de9d1-119">关系</span><span class="sxs-lookup"><span data-stu-id="de9d1-119">Relationships</span></span>
<span data-ttu-id="de9d1-120">无</span><span class="sxs-lookup"><span data-stu-id="de9d1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de9d1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de9d1-121">JSON Representation</span></span>
<span data-ttu-id="de9d1-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de9d1-122">Here is a JSON representation of the resource.</span></span>
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





