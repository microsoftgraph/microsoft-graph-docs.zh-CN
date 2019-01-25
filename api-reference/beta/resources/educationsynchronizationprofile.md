---
title: educationSynchronizationProfile 资源类型
description: 代表一组配置用于同步教育实体和 Azure Active Directory (Azure AD) 从源目录名单信息。 此资源提供了用于学校数据同步的编程表示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e1b81ff14aca2b0f81a7f50e01aed6281d03d14d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523461"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="76234-104">educationSynchronizationProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="76234-104">educationSynchronizationProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76234-105">代表一组配置用于同步教育实体和 Azure Active Directory (Azure AD) 从源目录名单信息。</span><span class="sxs-lookup"><span data-stu-id="76234-105">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="76234-106">此资源提供了用于[学校数据同步](https://sds.microsoft.com)的编程表示。</span><span class="sxs-lookup"><span data-stu-id="76234-106">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="76234-107">方法</span><span class="sxs-lookup"><span data-stu-id="76234-107">Methods</span></span>

| <span data-ttu-id="76234-108">方法</span><span class="sxs-lookup"><span data-stu-id="76234-108">Method</span></span> | <span data-ttu-id="76234-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="76234-109">Return Type</span></span> | <span data-ttu-id="76234-110">说明</span><span class="sxs-lookup"><span data-stu-id="76234-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="76234-111">列表同步配置文件</span><span class="sxs-lookup"><span data-stu-id="76234-111">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md) | <span data-ttu-id="76234-112">**educationSynchronizationProfile**集合</span><span class="sxs-lookup"><span data-stu-id="76234-112">**educationSynchronizationProfile** collection</span></span> | <span data-ttu-id="76234-113">获取为租户中的所有同步配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="76234-113">Get a list of all the synchronization profiles in the tenant.</span></span> |
| [<span data-ttu-id="76234-114">获取同步配置文件</span><span class="sxs-lookup"><span data-stu-id="76234-114">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md) | <span data-ttu-id="76234-115">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="76234-115">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="76234-116">检索给定的配置文件标识符特定配置文件。</span><span class="sxs-lookup"><span data-stu-id="76234-116">Retrieve a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="76234-117">创建同步配置文件</span><span class="sxs-lookup"><span data-stu-id="76234-117">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md) | <span data-ttu-id="76234-118">无</span><span class="sxs-lookup"><span data-stu-id="76234-118">None</span></span> | <span data-ttu-id="76234-119">创建一个新的同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="76234-119">Create a new synchronization profile.</span></span> |
| [<span data-ttu-id="76234-120">删除同步配置文件</span><span class="sxs-lookup"><span data-stu-id="76234-120">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md) | <span data-ttu-id="76234-121">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="76234-121">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="76234-122">删除特定的配置文件给定的配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="76234-122">Delete a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="76234-123">暂停正在进行同步</span><span class="sxs-lookup"><span data-stu-id="76234-123">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md) | <span data-ttu-id="76234-124">无</span><span class="sxs-lookup"><span data-stu-id="76234-124">None</span></span> | <span data-ttu-id="76234-125">暂停正在进行的同步。</span><span class="sxs-lookup"><span data-stu-id="76234-125">Pause an ongoing synchronization.</span></span> |
| [<span data-ttu-id="76234-126">恢复暂停的同步</span><span class="sxs-lookup"><span data-stu-id="76234-126">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md) | <span data-ttu-id="76234-127">无</span><span class="sxs-lookup"><span data-stu-id="76234-127">None</span></span> | <span data-ttu-id="76234-128">恢复暂停的同步。</span><span class="sxs-lookup"><span data-stu-id="76234-128">Resume a paused synchronization.</span></span> |
| [<span data-ttu-id="76234-129">重置 sync</span><span class="sxs-lookup"><span data-stu-id="76234-129">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md) | <span data-ttu-id="76234-130">无</span><span class="sxs-lookup"><span data-stu-id="76234-130">None</span></span> | <span data-ttu-id="76234-131">重置配置文件的状态，并重新启动同步。</span><span class="sxs-lookup"><span data-stu-id="76234-131">Reset the state of the profile and restart synchronization.</span></span> |
| [<span data-ttu-id="76234-132">启动同步上载文件</span><span class="sxs-lookup"><span data-stu-id="76234-132">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) | <span data-ttu-id="76234-133">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)集合</span><span class="sxs-lookup"><span data-stu-id="76234-133">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md) collection</span></span>| <span data-ttu-id="76234-134">验证已上载的源文件，并启动同步。</span><span class="sxs-lookup"><span data-stu-id="76234-134">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="76234-135">应用仅数据提供程序何时[educationCsvDataProvider](educationcsvdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="76234-135">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="76234-136">获取一个上载 URL</span><span class="sxs-lookup"><span data-stu-id="76234-136">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="76234-137">string</span><span class="sxs-lookup"><span data-stu-id="76234-137">string</span></span> | <span data-ttu-id="76234-138">返回要上载 CSV 数据文件的短期 URL。</span><span class="sxs-lookup"><span data-stu-id="76234-138">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="76234-139">应用仅数据提供程序何时[educationCsvDataProvider](educationcsvdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="76234-139">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="76234-140">要获取同步的状态</span><span class="sxs-lookup"><span data-stu-id="76234-140">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | [<span data-ttu-id="76234-141">status</span><span class="sxs-lookup"><span data-stu-id="76234-141">status</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="76234-142">返回一个特定的同步配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="76234-142">Return the status of a specific synchronization profile.</span></span> |
| [<span data-ttu-id="76234-143">获取同步错误</span><span class="sxs-lookup"><span data-stu-id="76234-143">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="76234-144">[educationSynchronizationError](educationsynchronizationerror.md)集合</span><span class="sxs-lookup"><span data-stu-id="76234-144">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="76234-145">获取所有同步过程中生成的错误。</span><span class="sxs-lookup"><span data-stu-id="76234-145">Get all the errors generated during synchronization.</span></span> |

## <a name="properties"></a><span data-ttu-id="76234-146">属性</span><span class="sxs-lookup"><span data-stu-id="76234-146">Properties</span></span>

| <span data-ttu-id="76234-147">属性</span><span class="sxs-lookup"><span data-stu-id="76234-147">Property</span></span> | <span data-ttu-id="76234-148">类型</span><span class="sxs-lookup"><span data-stu-id="76234-148">Type</span></span> | <span data-ttu-id="76234-149">说明</span><span class="sxs-lookup"><span data-stu-id="76234-149">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="76234-150">**displayName**</span><span class="sxs-lookup"><span data-stu-id="76234-150">**displayName**</span></span> | <span data-ttu-id="76234-151">string</span><span class="sxs-lookup"><span data-stu-id="76234-151">string</span></span> |  <span data-ttu-id="76234-152">配置文件的同步标识名称。</span><span class="sxs-lookup"><span data-stu-id="76234-152">Name of the configuration profile for syncing identities.</span></span>         |
| <span data-ttu-id="76234-153">**dataProvider**</span><span class="sxs-lookup"><span data-stu-id="76234-153">**dataProvider**</span></span> | [<span data-ttu-id="76234-154">educationSynchronizationDataProvider</span><span class="sxs-lookup"><span data-stu-id="76234-154">educationSynchronizationDataProvider</span></span>](educationsynchronizationdataprovider.md) |  <span data-ttu-id="76234-155">用于配置文件数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="76234-155">The data provider used for the profile.</span></span>         |
| <span data-ttu-id="76234-156">**identitySynchronizationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="76234-156">**identitySynchronizationConfiguration**</span></span> | [<span data-ttu-id="76234-157">educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="76234-157">educationIdentitySynchronizationConfiguration</span></span>](educationidentitysynchronizationconfiguration.md) | <span data-ttu-id="76234-158">标识[创建](educationidentitycreationconfiguration.md)或[匹配](educationidentitymatchingconfiguration.md)配置。</span><span class="sxs-lookup"><span data-stu-id="76234-158">Identity [creation](educationidentitycreationconfiguration.md) or [matching](educationidentitymatchingconfiguration.md) configuration .</span></span>        |
| <span data-ttu-id="76234-159">**licensesToAssign**</span><span class="sxs-lookup"><span data-stu-id="76234-159">**licensesToAssign**</span></span> | <span data-ttu-id="76234-160">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="76234-160">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md) collection</span></span>|  <span data-ttu-id="76234-161">许可证安装配置。</span><span class="sxs-lookup"><span data-stu-id="76234-161">License setup configuration.</span></span>        |
| <span data-ttu-id="76234-162">**state**</span><span class="sxs-lookup"><span data-stu-id="76234-162">**state**</span></span> | <span data-ttu-id="76234-163">educationSynchronizationProfileState</span><span class="sxs-lookup"><span data-stu-id="76234-163">educationSynchronizationProfileState</span></span> |  <span data-ttu-id="76234-164">配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="76234-164">The state of the profile.</span></span> <span data-ttu-id="76234-165">可取值为：`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed`。</span><span class="sxs-lookup"><span data-stu-id="76234-165">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span>          |

## <a name="relationships"></a><span data-ttu-id="76234-166">关系</span><span class="sxs-lookup"><span data-stu-id="76234-166">Relationships</span></span>

| <span data-ttu-id="76234-167">属性</span><span class="sxs-lookup"><span data-stu-id="76234-167">Property</span></span> | <span data-ttu-id="76234-168">类型</span><span class="sxs-lookup"><span data-stu-id="76234-168">Type</span></span> | <span data-ttu-id="76234-169">说明</span><span class="sxs-lookup"><span data-stu-id="76234-169">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="76234-170">**errors**</span><span class="sxs-lookup"><span data-stu-id="76234-170">**errors**</span></span> | <span data-ttu-id="76234-171">[educationSynchronizationError](educationsynchronizationerror.md)集合</span><span class="sxs-lookup"><span data-stu-id="76234-171">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="76234-172">与此同步配置文件关联的所有错误。</span><span class="sxs-lookup"><span data-stu-id="76234-172">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="76234-173">**profileStatus**</span><span class="sxs-lookup"><span data-stu-id="76234-173">**profileStatus**</span></span> | [<span data-ttu-id="76234-174">educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="76234-174">educationSynchronizationProfileStatus</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="76234-175">同步状态。</span><span class="sxs-lookup"><span data-stu-id="76234-175">The synchronization status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76234-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76234-176">JSON representation</span></span>
<span data-ttu-id="76234-177">下面是**educationSynchronizationProfile**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76234-177">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
    "displayName": "String",
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "microsoft.graph.educationCsvDataProvider" },
    "identitySynchronizationConfiguration": { "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
