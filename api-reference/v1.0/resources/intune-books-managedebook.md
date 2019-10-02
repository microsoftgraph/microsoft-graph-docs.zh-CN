---
title: managedEBook 资源类型
description: 包含托管电子书基属性的抽象类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3288b86ec735b4480577bb36a604107a51bb4f7f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360459"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="76748-103">managedEBook 资源类型</span><span class="sxs-lookup"><span data-stu-id="76748-103">managedEBook resource type</span></span>

> <span data-ttu-id="76748-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76748-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76748-105">包含托管电子书基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="76748-105">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="76748-106">方法</span><span class="sxs-lookup"><span data-stu-id="76748-106">Methods</span></span>
|<span data-ttu-id="76748-107">方法</span><span class="sxs-lookup"><span data-stu-id="76748-107">Method</span></span>|<span data-ttu-id="76748-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="76748-108">Return Type</span></span>|<span data-ttu-id="76748-109">说明</span><span class="sxs-lookup"><span data-stu-id="76748-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="76748-110">List managedEBooks</span><span class="sxs-lookup"><span data-stu-id="76748-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="76748-111">[managedEBook](../resources/intune-books-managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="76748-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="76748-112">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76748-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="76748-113">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="76748-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="76748-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="76748-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="76748-115">读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76748-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="76748-116">assign 操作</span><span class="sxs-lookup"><span data-stu-id="76748-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="76748-117">无</span><span class="sxs-lookup"><span data-stu-id="76748-117">None</span></span>|<span data-ttu-id="76748-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="76748-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="76748-119">属性</span><span class="sxs-lookup"><span data-stu-id="76748-119">Properties</span></span>
|<span data-ttu-id="76748-120">属性</span><span class="sxs-lookup"><span data-stu-id="76748-120">Property</span></span>|<span data-ttu-id="76748-121">类型</span><span class="sxs-lookup"><span data-stu-id="76748-121">Type</span></span>|<span data-ttu-id="76748-122">说明</span><span class="sxs-lookup"><span data-stu-id="76748-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76748-123">id</span><span class="sxs-lookup"><span data-stu-id="76748-123">id</span></span>|<span data-ttu-id="76748-124">字符串</span><span class="sxs-lookup"><span data-stu-id="76748-124">String</span></span>|<span data-ttu-id="76748-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="76748-125">Key of the entity.</span></span>|
|<span data-ttu-id="76748-126">displayName</span><span class="sxs-lookup"><span data-stu-id="76748-126">displayName</span></span>|<span data-ttu-id="76748-127">字符串</span><span class="sxs-lookup"><span data-stu-id="76748-127">String</span></span>|<span data-ttu-id="76748-128">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="76748-128">Name of the eBook.</span></span>|
|<span data-ttu-id="76748-129">说明</span><span class="sxs-lookup"><span data-stu-id="76748-129">description</span></span>|<span data-ttu-id="76748-130">String</span><span class="sxs-lookup"><span data-stu-id="76748-130">String</span></span>|<span data-ttu-id="76748-131">说明。</span><span class="sxs-lookup"><span data-stu-id="76748-131">Description.</span></span>|
|<span data-ttu-id="76748-132">publisher</span><span class="sxs-lookup"><span data-stu-id="76748-132">publisher</span></span>|<span data-ttu-id="76748-133">String</span><span class="sxs-lookup"><span data-stu-id="76748-133">String</span></span>|<span data-ttu-id="76748-134">发布者。</span><span class="sxs-lookup"><span data-stu-id="76748-134">Publisher.</span></span>|
|<span data-ttu-id="76748-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="76748-135">publishedDateTime</span></span>|<span data-ttu-id="76748-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76748-136">DateTimeOffset</span></span>|<span data-ttu-id="76748-137">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="76748-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="76748-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="76748-138">largeCover</span></span>|[<span data-ttu-id="76748-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="76748-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="76748-140">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="76748-140">Book cover.</span></span>|
|<span data-ttu-id="76748-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76748-141">createdDateTime</span></span>|<span data-ttu-id="76748-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76748-142">DateTimeOffset</span></span>|<span data-ttu-id="76748-143">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="76748-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="76748-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76748-144">lastModifiedDateTime</span></span>|<span data-ttu-id="76748-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76748-145">DateTimeOffset</span></span>|<span data-ttu-id="76748-146">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="76748-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="76748-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="76748-147">informationUrl</span></span>|<span data-ttu-id="76748-148">String</span><span class="sxs-lookup"><span data-stu-id="76748-148">String</span></span>|<span data-ttu-id="76748-149">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="76748-149">The more information Url.</span></span>|
|<span data-ttu-id="76748-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="76748-150">privacyInformationUrl</span></span>|<span data-ttu-id="76748-151">String</span><span class="sxs-lookup"><span data-stu-id="76748-151">String</span></span>|<span data-ttu-id="76748-152">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="76748-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76748-153">关系</span><span class="sxs-lookup"><span data-stu-id="76748-153">Relationships</span></span>
|<span data-ttu-id="76748-154">关系</span><span class="sxs-lookup"><span data-stu-id="76748-154">Relationship</span></span>|<span data-ttu-id="76748-155">类型</span><span class="sxs-lookup"><span data-stu-id="76748-155">Type</span></span>|<span data-ttu-id="76748-156">说明</span><span class="sxs-lookup"><span data-stu-id="76748-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76748-157">assignments</span><span class="sxs-lookup"><span data-stu-id="76748-157">assignments</span></span>|<span data-ttu-id="76748-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="76748-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="76748-159">此电子书的分配列表。</span><span class="sxs-lookup"><span data-stu-id="76748-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="76748-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="76748-160">installSummary</span></span>|[<span data-ttu-id="76748-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="76748-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="76748-162">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="76748-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="76748-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="76748-163">deviceStates</span></span>|<span data-ttu-id="76748-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="76748-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="76748-165">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="76748-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="76748-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="76748-166">userStateSummary</span></span>|<span data-ttu-id="76748-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="76748-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="76748-168">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="76748-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76748-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76748-169">JSON Representation</span></span>
<span data-ttu-id="76748-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76748-170">Here is a JSON representation of the resource.</span></span>
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




