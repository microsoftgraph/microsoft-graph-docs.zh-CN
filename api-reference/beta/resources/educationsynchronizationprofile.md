---
title: educationSynchronizationProfile 资源类型
description: 表示一组用于将源目录中的教育实体和名单信息同步到 Azure Active Directory （Azure AD）的配置。 此资源提供在学校数据同步中使用的编程表示形式。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 86c8189e170bba5899f82f75902dfe68dd0d3fd1
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434908"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="088c3-104">educationSynchronizationProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="088c3-104">educationSynchronizationProfile resource type</span></span>

<span data-ttu-id="088c3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="088c3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="088c3-106">表示一组用于将源目录中的教育实体和名单信息同步到 Azure Active Directory （Azure AD）的配置。</span><span class="sxs-lookup"><span data-stu-id="088c3-106">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="088c3-107">此资源提供在[学校数据同步](https://sds.microsoft.com)中使用的编程表示形式。</span><span class="sxs-lookup"><span data-stu-id="088c3-107">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="088c3-108">方法</span><span class="sxs-lookup"><span data-stu-id="088c3-108">Methods</span></span>

| <span data-ttu-id="088c3-109">方法</span><span class="sxs-lookup"><span data-stu-id="088c3-109">Method</span></span>                                                                    | <span data-ttu-id="088c3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="088c3-110">Return Type</span></span>                                                 | <span data-ttu-id="088c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="088c3-111">Description</span></span>                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="088c3-112">列出配置文件</span><span class="sxs-lookup"><span data-stu-id="088c3-112">List profiles</span></span>](../api/educationsynchronizationprofile-list.md)           | <span data-ttu-id="088c3-113">[educationSynchronizationProfile]集合</span><span class="sxs-lookup"><span data-stu-id="088c3-113">[educationSynchronizationProfile] collection</span></span>                | <span data-ttu-id="088c3-114">获取租户中所有同步配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="088c3-114">Get a list of all the synchronization profiles in the tenant.</span></span>                                                                  |
| [<span data-ttu-id="088c3-115">获取个人资料</span><span class="sxs-lookup"><span data-stu-id="088c3-115">Get profile</span></span>](../api/educationsynchronizationprofile-get.md)              | <span data-ttu-id="088c3-116">[educationSynchronizationProfile]</span><span class="sxs-lookup"><span data-stu-id="088c3-116">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="088c3-117">在给定配置文件标识符的情况检索特定配置文件。</span><span class="sxs-lookup"><span data-stu-id="088c3-117">Retrieve a specific profile given the profile identifier.</span></span>                                                                      |
| [<span data-ttu-id="088c3-118">创建配置文件</span><span class="sxs-lookup"><span data-stu-id="088c3-118">Create profile</span></span>](../api/educationsynchronizationprofile-post.md)          | <span data-ttu-id="088c3-119">无</span><span class="sxs-lookup"><span data-stu-id="088c3-119">None</span></span>                                                        | <span data-ttu-id="088c3-120">创建新的同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="088c3-120">Create a new synchronization profile.</span></span>                                                                                          |
| [<span data-ttu-id="088c3-121">删除个人资料</span><span class="sxs-lookup"><span data-stu-id="088c3-121">Delete profile</span></span>](../api/educationsynchronizationprofile-delete.md)        | <span data-ttu-id="088c3-122">[educationSynchronizationProfile]</span><span class="sxs-lookup"><span data-stu-id="088c3-122">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="088c3-123">在给定配置文件标识符的情况删除特定配置文件。</span><span class="sxs-lookup"><span data-stu-id="088c3-123">Delete a specific profile given the profile identifier.</span></span>                                                                        |
| [<span data-ttu-id="088c3-124">暂停配置文件</span><span class="sxs-lookup"><span data-stu-id="088c3-124">Pause profile</span></span>](../api/educationsynchronizationprofile-pause.md)          | <span data-ttu-id="088c3-125">无</span><span class="sxs-lookup"><span data-stu-id="088c3-125">None</span></span>                                                        | <span data-ttu-id="088c3-126">暂停正在进行的同步。</span><span class="sxs-lookup"><span data-stu-id="088c3-126">Pause an ongoing synchronization.</span></span>                                                                                              |
| [<span data-ttu-id="088c3-127">恢复配置文件</span><span class="sxs-lookup"><span data-stu-id="088c3-127">Resume profile</span></span>](../api/educationsynchronizationprofile-resume.md)        | <span data-ttu-id="088c3-128">无</span><span class="sxs-lookup"><span data-stu-id="088c3-128">None</span></span>                                                        | <span data-ttu-id="088c3-129">恢复暂停的同步。</span><span class="sxs-lookup"><span data-stu-id="088c3-129">Resume a paused synchronization.</span></span>                                                                                               |
| [<span data-ttu-id="088c3-130">重置配置文件</span><span class="sxs-lookup"><span data-stu-id="088c3-130">Reset profile</span></span>](../api/educationsynchronizationprofile-reset.md)          | <span data-ttu-id="088c3-131">无</span><span class="sxs-lookup"><span data-stu-id="088c3-131">None</span></span>                                                        | <span data-ttu-id="088c3-132">重置配置文件的状态并重新启动同步。</span><span class="sxs-lookup"><span data-stu-id="088c3-132">Reset the state of the profile and restart synchronization.</span></span>                                                                    |
| [<span data-ttu-id="088c3-133">启动 CSV 配置文件</span><span class="sxs-lookup"><span data-stu-id="088c3-133">Start CSV profile</span></span>](../api/educationsynchronizationprofile-start.md)      | <span data-ttu-id="088c3-134">[educationFileSynchronizationVerificationMessage]集合</span><span class="sxs-lookup"><span data-stu-id="088c3-134">[educationFileSynchronizationVerificationMessage]collection</span></span> | <span data-ttu-id="088c3-135">验证上载的源文件并启动同步。</span><span class="sxs-lookup"><span data-stu-id="088c3-135">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="088c3-136">仅在数据提供程序为[educationCsvDataProvider]时适用。</span><span class="sxs-lookup"><span data-stu-id="088c3-136">Applies only when the data provider is [educationCsvDataProvider].</span></span> |
| [<span data-ttu-id="088c3-137">获取 CSV 上载 URL</span><span class="sxs-lookup"><span data-stu-id="088c3-137">Get CSV upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="088c3-138">string</span><span class="sxs-lookup"><span data-stu-id="088c3-138">string</span></span>                                                      | <span data-ttu-id="088c3-139">返回短生存期的 URL 以上载 CSV 数据文件。</span><span class="sxs-lookup"><span data-stu-id="088c3-139">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="088c3-140">仅在数据提供程序为[educationCsvDataProvider]时适用。</span><span class="sxs-lookup"><span data-stu-id="088c3-140">Applies only when the data provider is [educationCsvDataProvider].</span></span>        |
| [<span data-ttu-id="088c3-141">获取状态</span><span class="sxs-lookup"><span data-stu-id="088c3-141">Get status</span></span>](../api/educationsynchronizationprofilestatus-get.md)         | <span data-ttu-id="088c3-142">[educationsynchronizationProfileStatus]</span><span class="sxs-lookup"><span data-stu-id="088c3-142">[educationsynchronizationProfileStatus]</span></span>                     | <span data-ttu-id="088c3-143">返回特定同步配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="088c3-143">Return the status of a specific synchronization profile.</span></span>                                                                       |
| [<span data-ttu-id="088c3-144">获取错误</span><span class="sxs-lookup"><span data-stu-id="088c3-144">Get errors</span></span>](../api/educationsynchronizationerrors-get.md)                | <span data-ttu-id="088c3-145">[educationSynchronizationError]集合</span><span class="sxs-lookup"><span data-stu-id="088c3-145">[educationSynchronizationError] collection</span></span>                  | <span data-ttu-id="088c3-146">获取同步过程中生成的所有错误。</span><span class="sxs-lookup"><span data-stu-id="088c3-146">Get all the errors generated during synchronization.</span></span>                                                                           |

## <a name="properties"></a><span data-ttu-id="088c3-147">属性</span><span class="sxs-lookup"><span data-stu-id="088c3-147">Properties</span></span>

| <span data-ttu-id="088c3-148">属性</span><span class="sxs-lookup"><span data-stu-id="088c3-148">Property</span></span>                             | <span data-ttu-id="088c3-149">类型</span><span class="sxs-lookup"><span data-stu-id="088c3-149">Type</span></span>                                                   | <span data-ttu-id="088c3-150">说明</span><span class="sxs-lookup"><span data-stu-id="088c3-150">Description</span></span>                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="088c3-151">id</span><span class="sxs-lookup"><span data-stu-id="088c3-151">id</span></span>                                   | <span data-ttu-id="088c3-152">字符串</span><span class="sxs-lookup"><span data-stu-id="088c3-152">String</span></span>                                                 | <span data-ttu-id="088c3-153">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="088c3-153">The unique identifier for the resource.</span></span> <span data-ttu-id="088c3-154">（只读）</span><span class="sxs-lookup"><span data-stu-id="088c3-154">(read-only)</span></span>                                                                               |
| <span data-ttu-id="088c3-155">displayName</span><span class="sxs-lookup"><span data-stu-id="088c3-155">displayName</span></span>                          | <span data-ttu-id="088c3-156">String</span><span class="sxs-lookup"><span data-stu-id="088c3-156">String</span></span>                                                 | <span data-ttu-id="088c3-157">用于同步标识的配置文件的名称。</span><span class="sxs-lookup"><span data-stu-id="088c3-157">Name of the configuration profile for syncing identities.</span></span>                                                                         |
| <span data-ttu-id="088c3-158">dataProvider</span><span class="sxs-lookup"><span data-stu-id="088c3-158">dataProvider</span></span>                         | <span data-ttu-id="088c3-159">[educationSynchronizationDataProvider]</span><span class="sxs-lookup"><span data-stu-id="088c3-159">[educationSynchronizationDataProvider]</span></span>                 | <span data-ttu-id="088c3-160">用于配置文件的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="088c3-160">The data provider used for the profile.</span></span>                                                                                           |
| <span data-ttu-id="088c3-161">expirationDate</span><span class="sxs-lookup"><span data-stu-id="088c3-161">expirationDate</span></span>                       | <span data-ttu-id="088c3-162">日期</span><span class="sxs-lookup"><span data-stu-id="088c3-162">Date</span></span>                                                   | <span data-ttu-id="088c3-163">应将配置文件视为已过期并停止同步的日期。</span><span class="sxs-lookup"><span data-stu-id="088c3-163">The date the profile should be considered expired and cease syncing.</span></span> <span data-ttu-id="088c3-164">When `null` 。</span><span class="sxs-lookup"><span data-stu-id="088c3-164">When `null`.</span></span> <span data-ttu-id="088c3-165">配置文件永远不会过期。</span><span class="sxs-lookup"><span data-stu-id="088c3-165">the profile will never expire.</span></span> <span data-ttu-id="088c3-166">（可选）</span><span class="sxs-lookup"><span data-stu-id="088c3-166">(optional)</span></span>       |
| <span data-ttu-id="088c3-167">handleSpecialCharacterConstraint</span><span class="sxs-lookup"><span data-stu-id="088c3-167">handleSpecialCharacterConstraint</span></span>     | <span data-ttu-id="088c3-168">Bool</span><span class="sxs-lookup"><span data-stu-id="088c3-168">Bool</span></span>                                                   | <span data-ttu-id="088c3-169">确定在从源同步时，学校数据同步是否应自动替换不受支持的特殊字符。</span><span class="sxs-lookup"><span data-stu-id="088c3-169">Determines if School Data Sync should automatically replace unsupported special characters while syncing from source.</span></span>             |
| <span data-ttu-id="088c3-170">identitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="088c3-170">identitySynchronizationConfiguration</span></span> | <span data-ttu-id="088c3-171">[educationIdentitySynchronizationConfiguration]</span><span class="sxs-lookup"><span data-stu-id="088c3-171">[educationIdentitySynchronizationConfiguration]</span></span>        | <span data-ttu-id="088c3-172">确定配置文件应如何[新建][fullsync]或[匹配现有][dirsync]AAD 用户。</span><span class="sxs-lookup"><span data-stu-id="088c3-172">Determines how the Profile should [create new][fullsync] or [match existing][dirsync] AAD Users.</span></span>                                  |
| <span data-ttu-id="088c3-173">licensesToAssign</span><span class="sxs-lookup"><span data-stu-id="088c3-173">licensesToAssign</span></span>                     | <span data-ttu-id="088c3-174">[educationSynchronizationLicenseAssignment]集合</span><span class="sxs-lookup"><span data-stu-id="088c3-174">[educationSynchronizationLicenseAssignment] collection</span></span> | <span data-ttu-id="088c3-175">许可证安装程序配置。</span><span class="sxs-lookup"><span data-stu-id="088c3-175">License setup configuration.</span></span>                                                                                                      |
| <span data-ttu-id="088c3-176">state</span><span class="sxs-lookup"><span data-stu-id="088c3-176">state</span></span>                                | <span data-ttu-id="088c3-177">educationSynchronizationProfileState</span><span class="sxs-lookup"><span data-stu-id="088c3-177">educationSynchronizationProfileState</span></span>                   | <span data-ttu-id="088c3-178">配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="088c3-178">The state of the profile.</span></span> <span data-ttu-id="088c3-179">可取值为：`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed`。</span><span class="sxs-lookup"><span data-stu-id="088c3-179">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="088c3-180">关系</span><span class="sxs-lookup"><span data-stu-id="088c3-180">Relationships</span></span>

| <span data-ttu-id="088c3-181">关系</span><span class="sxs-lookup"><span data-stu-id="088c3-181">Relationship</span></span>  | <span data-ttu-id="088c3-182">类型</span><span class="sxs-lookup"><span data-stu-id="088c3-182">Type</span></span>                                       | <span data-ttu-id="088c3-183">说明</span><span class="sxs-lookup"><span data-stu-id="088c3-183">Description</span></span>                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| <span data-ttu-id="088c3-184">错误</span><span class="sxs-lookup"><span data-stu-id="088c3-184">errors</span></span>        | <span data-ttu-id="088c3-185">[educationSynchronizationError]集合</span><span class="sxs-lookup"><span data-stu-id="088c3-185">[educationSynchronizationError] collection</span></span> | <span data-ttu-id="088c3-186">与此同步配置文件关联的所有错误。</span><span class="sxs-lookup"><span data-stu-id="088c3-186">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="088c3-187">profileStatus</span><span class="sxs-lookup"><span data-stu-id="088c3-187">profileStatus</span></span> | <span data-ttu-id="088c3-188">[educationSynchronizationProfileStatus]</span><span class="sxs-lookup"><span data-stu-id="088c3-188">[educationSynchronizationProfileStatus]</span></span>    | <span data-ttu-id="088c3-189">同步状态。</span><span class="sxs-lookup"><span data-stu-id="088c3-189">The synchronization status.</span></span>                              |

## <a name="data-providers"></a><span data-ttu-id="088c3-190">数据提供程序</span><span class="sxs-lookup"><span data-stu-id="088c3-190">Data Providers</span></span>

<span data-ttu-id="088c3-191">每个[educationSynchronizationProfile]必须指定要用作同步源的以下数据提供程序之一。</span><span class="sxs-lookup"><span data-stu-id="088c3-191">Each [educationSynchronizationProfile] must specify one of the follow data providers to use as the synchronization source.</span></span>

| <span data-ttu-id="088c3-192">Data Provider</span><span class="sxs-lookup"><span data-stu-id="088c3-192">Data Provider</span></span>                                                             | <span data-ttu-id="088c3-193">说明</span><span class="sxs-lookup"><span data-stu-id="088c3-193">Description</span></span>                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="088c3-194">[educationCsvDataProvider]</span><span class="sxs-lookup"><span data-stu-id="088c3-194">[educationCsvDataProvider]</span></span>                                                | <span data-ttu-id="088c3-195">上载到配置文件的[SAS URL](../api/educationsynchronizationprofile-uploadurl.md)的 CSV 文件</span><span class="sxs-lookup"><span data-stu-id="088c3-195">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="088c3-196">educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="088c3-196">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="088c3-197">OneRoster v1.1 API</span><span class="sxs-lookup"><span data-stu-id="088c3-197">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="088c3-198">[educationPowerSchoolDataProvider]</span><span class="sxs-lookup"><span data-stu-id="088c3-198">[educationPowerSchoolDataProvider]</span></span>                                        | <span data-ttu-id="088c3-199">PowerSchool API</span><span class="sxs-lookup"><span data-stu-id="088c3-199">PowerSchool API</span></span>                                                                                    |

## <a name="json-representation"></a><span data-ttu-id="088c3-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="088c3-200">JSON representation</span></span>

<span data-ttu-id="088c3-201">下面是**educationSynchronizationProfile**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="088c3-201">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "state": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileState"
  },
  "profileStatus": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
  },
  "errors": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
    }
  ],
  "dataProvider": {
    "@odata.type": "microsoft.graph.educationCsvDataProvider"
  },
  "identitySynchronizationConfiguration": {
    "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
  },
  "licensesToAssign": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
    }
  ],
  "handleSpecialCharacterConstraint": "Boolean",
  "expirationDate": "Date"
}
```

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationsynchronizationprofilestatus]: educationsynchronizationProfileStatus.md
[educationsynchronizationerror]: educationSynchronizationError.md
[educationfilesynchronizationverificationmessage]: educationFileSynchronizationVerificationMessage.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationidentitysynchronizationconfiguration]: educationIdentitySynchronizationConfiguration.md
[educationsynchronizationlicenseassignment]: educationSynchronizationLicenseAssignment.md
[fullsync]: educationidentitycreationconfiguration.md
[dirsync]: educationidentitycreationconfiguration.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSynchronizationProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationSynchronizationProfile/dataProvider:\r\n      Referenced type microsoft.graph.educationSynchronizationDataProvider is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
