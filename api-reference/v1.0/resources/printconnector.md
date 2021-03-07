---
title: printConnector 资源类型
description: 表示已使用通用打印订阅注册的打印连接器。 printConnector 资源可用于查看连接器状态和更新属性。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: e791ca755b695fc8e4704b65aff98a9db934d901
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517197"
---
# <a name="printconnector-resource-type"></a><span data-ttu-id="4b851-104">printConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b851-104">printConnector resource type</span></span>

<span data-ttu-id="4b851-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b851-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="4b851-106">表示已使用通用打印订阅注册的打印连接器。</span><span class="sxs-lookup"><span data-stu-id="4b851-106">Represents a print connector that has been registered by using a Universal Print subscription.</span></span> <span data-ttu-id="4b851-107">printConnector 资源可用于查看连接器状态和更新属性。</span><span class="sxs-lookup"><span data-stu-id="4b851-107">The printConnector resource can be used to view connector status and update properties.</span></span>

## <a name="methods"></a><span data-ttu-id="4b851-108">Methods</span><span class="sxs-lookup"><span data-stu-id="4b851-108">Methods</span></span>
|<span data-ttu-id="4b851-109">方法</span><span class="sxs-lookup"><span data-stu-id="4b851-109">Method</span></span>|<span data-ttu-id="4b851-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4b851-110">Return type</span></span>|<span data-ttu-id="4b851-111">Description</span><span class="sxs-lookup"><span data-stu-id="4b851-111">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="4b851-112">Get connector</span><span class="sxs-lookup"><span data-stu-id="4b851-112">Get connector</span></span>](../api/printconnector-get.md) | [<span data-ttu-id="4b851-113">printConnector</span><span class="sxs-lookup"><span data-stu-id="4b851-113">printConnector</span></span>](printconnector.md) | <span data-ttu-id="4b851-114">读取连接器对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b851-114">Read the properties and relationships of the connector object.</span></span> |
| [<span data-ttu-id="4b851-115">更新连接器</span><span class="sxs-lookup"><span data-stu-id="4b851-115">Update connector</span></span>](../api/printconnector-update.md) | [<span data-ttu-id="4b851-116">printConnector</span><span class="sxs-lookup"><span data-stu-id="4b851-116">printConnector</span></span>](printconnector.md) | <span data-ttu-id="4b851-117">更新连接器对象。</span><span class="sxs-lookup"><span data-stu-id="4b851-117">Update the connector object.</span></span> |
| [<span data-ttu-id="4b851-118">删除连接器</span><span class="sxs-lookup"><span data-stu-id="4b851-118">Delete connector</span></span>](../api/printconnector-delete.md) | <span data-ttu-id="4b851-119">无</span><span class="sxs-lookup"><span data-stu-id="4b851-119">None</span></span> | <span data-ttu-id="4b851-120">从通用打印服务中注销连接器。</span><span class="sxs-lookup"><span data-stu-id="4b851-120">Unregister the connector from the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="4b851-121">属性</span><span class="sxs-lookup"><span data-stu-id="4b851-121">Properties</span></span>
|<span data-ttu-id="4b851-122">属性</span><span class="sxs-lookup"><span data-stu-id="4b851-122">Property</span></span>|<span data-ttu-id="4b851-123">类型</span><span class="sxs-lookup"><span data-stu-id="4b851-123">Type</span></span>|<span data-ttu-id="4b851-124">说明</span><span class="sxs-lookup"><span data-stu-id="4b851-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b851-125">id</span><span class="sxs-lookup"><span data-stu-id="4b851-125">id</span></span>|<span data-ttu-id="4b851-126">String</span><span class="sxs-lookup"><span data-stu-id="4b851-126">String</span></span>| <span data-ttu-id="4b851-127">只读。</span><span class="sxs-lookup"><span data-stu-id="4b851-127">Read-only.</span></span>|
|<span data-ttu-id="4b851-128">displayName</span><span class="sxs-lookup"><span data-stu-id="4b851-128">displayName</span></span>|<span data-ttu-id="4b851-129">String</span><span class="sxs-lookup"><span data-stu-id="4b851-129">String</span></span>|<span data-ttu-id="4b851-130">连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="4b851-130">The name of the connector.</span></span>|
|<span data-ttu-id="4b851-131">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="4b851-131">fullyQualifiedDomainName</span></span>|<span data-ttu-id="4b851-132">String</span><span class="sxs-lookup"><span data-stu-id="4b851-132">String</span></span>|<span data-ttu-id="4b851-133">连接器计算机主机名。</span><span class="sxs-lookup"><span data-stu-id="4b851-133">The connector machine's hostname.</span></span>|
|<span data-ttu-id="4b851-134">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="4b851-134">operatingSystem</span></span>|<span data-ttu-id="4b851-135">String</span><span class="sxs-lookup"><span data-stu-id="4b851-135">String</span></span>|<span data-ttu-id="4b851-136">连接器计算机的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4b851-136">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="4b851-137">appVersion</span><span class="sxs-lookup"><span data-stu-id="4b851-137">appVersion</span></span>|<span data-ttu-id="4b851-138">String</span><span class="sxs-lookup"><span data-stu-id="4b851-138">String</span></span>|<span data-ttu-id="4b851-139">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="4b851-139">The connector's version.</span></span>|
|<span data-ttu-id="4b851-140">位置</span><span class="sxs-lookup"><span data-stu-id="4b851-140">location</span></span>|[<span data-ttu-id="4b851-141">printerLocation</span><span class="sxs-lookup"><span data-stu-id="4b851-141">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="4b851-142">连接器的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="4b851-142">The physical and/or organizational location of the connector.</span></span>|
|<span data-ttu-id="4b851-143">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="4b851-143">registeredDateTime</span></span>|<span data-ttu-id="4b851-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b851-144">DateTimeOffset</span></span>|<span data-ttu-id="4b851-145">连接器注册时的日期/时间Offset。</span><span class="sxs-lookup"><span data-stu-id="4b851-145">The DateTimeOffset when the connector was registered.</span></span>|
|<span data-ttu-id="4b851-146">registeredBy</span><span class="sxs-lookup"><span data-stu-id="4b851-146">registeredBy</span></span>|[<span data-ttu-id="4b851-147">userIdentity</span><span class="sxs-lookup"><span data-stu-id="4b851-147">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="4b851-148">注册连接器的用户。</span><span class="sxs-lookup"><span data-stu-id="4b851-148">The user who registered the connector.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b851-149">关系</span><span class="sxs-lookup"><span data-stu-id="4b851-149">Relationships</span></span>
<span data-ttu-id="4b851-150">无。</span><span class="sxs-lookup"><span data-stu-id="4b851-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b851-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b851-151">JSON representation</span></span>
<span data-ttu-id="4b851-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b851-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printConnector",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "registeredDateTime": "String (timestamp)"
}
```