---
title: printConnector 资源类型
description: 表示已使用通用打印订阅注册的打印连接器。 PrintConnector 资源可用于查看连接器状态和更新属性。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7c66933c381e2f7563f4666ca788d06970b04490
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895632"
---
# <a name="printconnector-resource-type"></a><span data-ttu-id="23c35-104">printConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="23c35-104">printConnector resource type</span></span>

<span data-ttu-id="23c35-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23c35-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23c35-106">表示已使用通用打印订阅注册的打印连接器。</span><span class="sxs-lookup"><span data-stu-id="23c35-106">Represents a print connector that has been registered by using a Universal Print subscription.</span></span> <span data-ttu-id="23c35-107">PrintConnector 资源可用于查看连接器状态和更新属性。</span><span class="sxs-lookup"><span data-stu-id="23c35-107">The printConnector resource can be used to view connector status and update properties.</span></span>

## <a name="methods"></a><span data-ttu-id="23c35-108">方法</span><span class="sxs-lookup"><span data-stu-id="23c35-108">Methods</span></span>

| <span data-ttu-id="23c35-109">方法</span><span class="sxs-lookup"><span data-stu-id="23c35-109">Method</span></span>       | <span data-ttu-id="23c35-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="23c35-110">Return Type</span></span> | <span data-ttu-id="23c35-111">说明</span><span class="sxs-lookup"><span data-stu-id="23c35-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="23c35-112">获取连接器</span><span class="sxs-lookup"><span data-stu-id="23c35-112">Get connector</span></span>](../api/printconnector-get.md) | [<span data-ttu-id="23c35-113">printConnector</span><span class="sxs-lookup"><span data-stu-id="23c35-113">printConnector</span></span>](printconnector.md) | <span data-ttu-id="23c35-114">读取连接器对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23c35-114">Read the properties and relationships of the connector object.</span></span> |
| [<span data-ttu-id="23c35-115">更新连接器</span><span class="sxs-lookup"><span data-stu-id="23c35-115">Update connector</span></span>](../api/printconnector-update.md) | [<span data-ttu-id="23c35-116">printConnector</span><span class="sxs-lookup"><span data-stu-id="23c35-116">printConnector</span></span>](printconnector.md) | <span data-ttu-id="23c35-117">更新连接器对象。</span><span class="sxs-lookup"><span data-stu-id="23c35-117">Update the connector object.</span></span> |
| [<span data-ttu-id="23c35-118">删除连接器</span><span class="sxs-lookup"><span data-stu-id="23c35-118">Delete connector</span></span>](../api/printconnector-delete.md) | <span data-ttu-id="23c35-119">无</span><span class="sxs-lookup"><span data-stu-id="23c35-119">None</span></span> | <span data-ttu-id="23c35-120">从通用打印服务中注销连接器。</span><span class="sxs-lookup"><span data-stu-id="23c35-120">Unregister the connector from the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="23c35-121">属性</span><span class="sxs-lookup"><span data-stu-id="23c35-121">Properties</span></span>
| <span data-ttu-id="23c35-122">属性</span><span class="sxs-lookup"><span data-stu-id="23c35-122">Property</span></span>     | <span data-ttu-id="23c35-123">类型</span><span class="sxs-lookup"><span data-stu-id="23c35-123">Type</span></span>        | <span data-ttu-id="23c35-124">说明</span><span class="sxs-lookup"><span data-stu-id="23c35-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23c35-125">id</span><span class="sxs-lookup"><span data-stu-id="23c35-125">id</span></span>|<span data-ttu-id="23c35-126">String</span><span class="sxs-lookup"><span data-stu-id="23c35-126">String</span></span>| <span data-ttu-id="23c35-127">只读。</span><span class="sxs-lookup"><span data-stu-id="23c35-127">Read-only.</span></span>|
|<span data-ttu-id="23c35-128">name</span><span class="sxs-lookup"><span data-stu-id="23c35-128">name</span></span>|<span data-ttu-id="23c35-129">String</span><span class="sxs-lookup"><span data-stu-id="23c35-129">String</span></span>|<span data-ttu-id="23c35-130">连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="23c35-130">The name of the connector.</span></span>|
|<span data-ttu-id="23c35-131">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="23c35-131">fullyQualifiedDomainName</span></span>|<span data-ttu-id="23c35-132">String</span><span class="sxs-lookup"><span data-stu-id="23c35-132">String</span></span>|<span data-ttu-id="23c35-133">连接器计算机的主机名。</span><span class="sxs-lookup"><span data-stu-id="23c35-133">The connector machine's hostname.</span></span>|
|<span data-ttu-id="23c35-134">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="23c35-134">operatingSystem</span></span>|<span data-ttu-id="23c35-135">String</span><span class="sxs-lookup"><span data-stu-id="23c35-135">String</span></span>|<span data-ttu-id="23c35-136">连接器计算机的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="23c35-136">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="23c35-137">appVersion</span><span class="sxs-lookup"><span data-stu-id="23c35-137">appVersion</span></span>|<span data-ttu-id="23c35-138">String</span><span class="sxs-lookup"><span data-stu-id="23c35-138">String</span></span>|<span data-ttu-id="23c35-139">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="23c35-139">The connector's version.</span></span>|
|<span data-ttu-id="23c35-140">deviceHealth</span><span class="sxs-lookup"><span data-stu-id="23c35-140">deviceHealth</span></span>|[<span data-ttu-id="23c35-141">deviceHealth</span><span class="sxs-lookup"><span data-stu-id="23c35-141">deviceHealth</span></span>](devicehealth.md)|<span data-ttu-id="23c35-142">连接器的设备运行状况。</span><span class="sxs-lookup"><span data-stu-id="23c35-142">The connector's device health.</span></span>|
|<span data-ttu-id="23c35-143">位置</span><span class="sxs-lookup"><span data-stu-id="23c35-143">location</span></span>|[<span data-ttu-id="23c35-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="23c35-144">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="23c35-145">连接器的物理位置和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="23c35-145">The physical and/or organizational location of the connector.</span></span>|
|<span data-ttu-id="23c35-146">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="23c35-146">registeredDateTime</span></span>|<span data-ttu-id="23c35-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23c35-147">DateTimeOffset</span></span>|<span data-ttu-id="23c35-148">注册连接器时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="23c35-148">The DateTimeOffset when the connector was registered.</span></span>|
|<span data-ttu-id="23c35-149">registeredBy</span><span class="sxs-lookup"><span data-stu-id="23c35-149">registeredBy</span></span>|[<span data-ttu-id="23c35-150">userIdentity</span><span class="sxs-lookup"><span data-stu-id="23c35-150">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="23c35-151">注册了连接器的用户。</span><span class="sxs-lookup"><span data-stu-id="23c35-151">The user who registered the connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23c35-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23c35-152">JSON representation</span></span>

<span data-ttu-id="23c35-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23c35-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printConnector"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "deviceHealth": {"@odata.type": "microsoft.graph.deviceHealth"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "registeredDateTime": "String (timestamp)",
  "registeredBy": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printConnector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->