---
title: managedEBook 资源类型
description: 包含托管电子书基属性的抽象类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 66d0efae21a68bd14286af45c4c021dbf7ba96fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531007"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="a5c52-103">managedEBook 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5c52-103">managedEBook resource type</span></span>

<span data-ttu-id="a5c52-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5c52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5c52-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5c52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5c52-106">包含托管电子书基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="a5c52-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="a5c52-107">Methods</span><span class="sxs-lookup"><span data-stu-id="a5c52-107">Methods</span></span>
|<span data-ttu-id="a5c52-108">方法</span><span class="sxs-lookup"><span data-stu-id="a5c52-108">Method</span></span>|<span data-ttu-id="a5c52-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a5c52-109">Return Type</span></span>|<span data-ttu-id="a5c52-110">说明</span><span class="sxs-lookup"><span data-stu-id="a5c52-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a5c52-111">List managedEBooks</span><span class="sxs-lookup"><span data-stu-id="a5c52-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="a5c52-112">[managedEBook](../resources/intune-books-managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a5c52-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="a5c52-113">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a5c52-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="a5c52-114">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="a5c52-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="a5c52-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="a5c52-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="a5c52-116">读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a5c52-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="a5c52-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="a5c52-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="a5c52-118">无</span><span class="sxs-lookup"><span data-stu-id="a5c52-118">None</span></span>|<span data-ttu-id="a5c52-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a5c52-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a5c52-120">属性</span><span class="sxs-lookup"><span data-stu-id="a5c52-120">Properties</span></span>
|<span data-ttu-id="a5c52-121">属性</span><span class="sxs-lookup"><span data-stu-id="a5c52-121">Property</span></span>|<span data-ttu-id="a5c52-122">类型</span><span class="sxs-lookup"><span data-stu-id="a5c52-122">Type</span></span>|<span data-ttu-id="a5c52-123">说明</span><span class="sxs-lookup"><span data-stu-id="a5c52-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5c52-124">id</span><span class="sxs-lookup"><span data-stu-id="a5c52-124">id</span></span>|<span data-ttu-id="a5c52-125">字符串</span><span class="sxs-lookup"><span data-stu-id="a5c52-125">String</span></span>|<span data-ttu-id="a5c52-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a5c52-126">Key of the entity.</span></span>|
|<span data-ttu-id="a5c52-127">displayName</span><span class="sxs-lookup"><span data-stu-id="a5c52-127">displayName</span></span>|<span data-ttu-id="a5c52-128">字符串</span><span class="sxs-lookup"><span data-stu-id="a5c52-128">String</span></span>|<span data-ttu-id="a5c52-129">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="a5c52-129">Name of the eBook.</span></span>|
|<span data-ttu-id="a5c52-130">说明</span><span class="sxs-lookup"><span data-stu-id="a5c52-130">description</span></span>|<span data-ttu-id="a5c52-131">String</span><span class="sxs-lookup"><span data-stu-id="a5c52-131">String</span></span>|<span data-ttu-id="a5c52-132">说明。</span><span class="sxs-lookup"><span data-stu-id="a5c52-132">Description.</span></span>|
|<span data-ttu-id="a5c52-133">publisher</span><span class="sxs-lookup"><span data-stu-id="a5c52-133">publisher</span></span>|<span data-ttu-id="a5c52-134">String</span><span class="sxs-lookup"><span data-stu-id="a5c52-134">String</span></span>|<span data-ttu-id="a5c52-135">发布者。</span><span class="sxs-lookup"><span data-stu-id="a5c52-135">Publisher.</span></span>|
|<span data-ttu-id="a5c52-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5c52-136">publishedDateTime</span></span>|<span data-ttu-id="a5c52-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5c52-137">DateTimeOffset</span></span>|<span data-ttu-id="a5c52-138">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a5c52-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="a5c52-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="a5c52-139">largeCover</span></span>|[<span data-ttu-id="a5c52-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a5c52-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a5c52-141">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="a5c52-141">Book cover.</span></span>|
|<span data-ttu-id="a5c52-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5c52-142">createdDateTime</span></span>|<span data-ttu-id="a5c52-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5c52-143">DateTimeOffset</span></span>|<span data-ttu-id="a5c52-144">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a5c52-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="a5c52-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5c52-145">lastModifiedDateTime</span></span>|<span data-ttu-id="a5c52-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5c52-146">DateTimeOffset</span></span>|<span data-ttu-id="a5c52-147">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a5c52-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="a5c52-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a5c52-148">informationUrl</span></span>|<span data-ttu-id="a5c52-149">String</span><span class="sxs-lookup"><span data-stu-id="a5c52-149">String</span></span>|<span data-ttu-id="a5c52-150">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="a5c52-150">The more information Url.</span></span>|
|<span data-ttu-id="a5c52-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a5c52-151">privacyInformationUrl</span></span>|<span data-ttu-id="a5c52-152">字符串</span><span class="sxs-lookup"><span data-stu-id="a5c52-152">String</span></span>|<span data-ttu-id="a5c52-153">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="a5c52-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5c52-154">关系</span><span class="sxs-lookup"><span data-stu-id="a5c52-154">Relationships</span></span>
|<span data-ttu-id="a5c52-155">关系</span><span class="sxs-lookup"><span data-stu-id="a5c52-155">Relationship</span></span>|<span data-ttu-id="a5c52-156">类型</span><span class="sxs-lookup"><span data-stu-id="a5c52-156">Type</span></span>|<span data-ttu-id="a5c52-157">说明</span><span class="sxs-lookup"><span data-stu-id="a5c52-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5c52-158">assignments</span><span class="sxs-lookup"><span data-stu-id="a5c52-158">assignments</span></span>|<span data-ttu-id="a5c52-159">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a5c52-159">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="a5c52-160">此电子书的分配列表。</span><span class="sxs-lookup"><span data-stu-id="a5c52-160">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="a5c52-161">installSummary</span><span class="sxs-lookup"><span data-stu-id="a5c52-161">installSummary</span></span>|[<span data-ttu-id="a5c52-162">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a5c52-162">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="a5c52-163">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="a5c52-163">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="a5c52-164">deviceStates</span><span class="sxs-lookup"><span data-stu-id="a5c52-164">deviceStates</span></span>|<span data-ttu-id="a5c52-165">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a5c52-165">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="a5c52-166">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="a5c52-166">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="a5c52-167">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="a5c52-167">userStateSummary</span></span>|<span data-ttu-id="a5c52-168">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a5c52-168">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="a5c52-169">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="a5c52-169">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5c52-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5c52-170">JSON Representation</span></span>
<span data-ttu-id="a5c52-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5c52-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```




