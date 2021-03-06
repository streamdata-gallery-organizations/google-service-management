---
name: Google Service Management
x-slug: google-service-management
description: Google Service Management is an infrastructure service of Google Cloud
  Platform that manages other APIs and services, including Googles own Cloud Platform
  services and their APIs, and services created using Google Cloud Endpoints.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Google Service Management
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/apis.md
specificationVersion: "0.14"
apis:
- name: Google Service Management - Get Services
  x-api-slug: v1services-get
  description: |-
    Lists managed services.

    Returns all public services. For authenticated users, also returns all
    services the calling user has "servicemanagement.services.get" permission
    for.

    **BETA:** If the caller specifies the `consumer_id`, it returns only the
    services enabled on the consumer. The `consumer_id` must have the format
    of "project:{PROJECT-ID}".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1services-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1services-get-openapi.md
- name: Google Service Management - Create Service
  x-api-slug: v1services-post
  description: |-
    Creates a new managed service.
    Please note one producer project can own no more than 20 services.

    Operation<response: ManagedService>
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1services-post-openapi.md
- name: Google Service Management - Delete Service
  x-api-slug: v1servicesservicename-delete
  description: |-
    Deletes a managed service. This method will change the service to the
    `Soft-Delete` state for 30 days. Within this period, service producers may
    call UndeleteService to restore the service.
    After 30 days, the service will be permanently deleted.

    Operation<response: google.protobuf.Empty>
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicename-delete-openapi.md
- name: Google Service Management - Get Service
  x-api-slug: v1servicesservicename-get
  description: |-
    Gets a managed service. Authentication is required unless the service is
    public.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicename-get-openapi.md
- name: Google Service Management - Create Service Configuration
  x-api-slug: v1servicesservicenameconfig-get
  description: Gets a service configuration (version) for a managed service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicenameconfig-get-openapi.md
- name: Google Service Management - Create Service Configurations
  x-api-slug: v1servicesservicenameconfigs-get
  description: |-
    Lists the history of the service configuration for a managed service,
    from the newest to the oldest.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicenameconfigs-get-openapi.md
- name: Google Service Management - Create Service Configuration
  x-api-slug: v1servicesservicenameconfigs-post
  description: |-
    Creates a new service configuration (version) for a managed service.
    This method only stores the service configuration. To roll out the service
    configuration to backend systems please call
    CreateServiceRollout.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicenameconfigs-post-openapi.md
- name: Google Service Management - Get Service Configuration
  x-api-slug: v1servicesservicenameconfigsconfigid-get
  description: Gets a service configuration (version) for a managed service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicenameconfigsconfigid-get-openapi.md
- name: Google Service Management - Create Service Configuration
  x-api-slug: v1servicesservicenameconfigssubmit-post
  description: |-
    Creates a new service configuration (version) for a managed service based
    on
    user-supplied configuration source files (for example: OpenAPI
    Specification). This method stores the source configurations as well as the
    generated service configuration. To rollout the service configuration to
    other services,
    please call CreateServiceRollout.

    Operation<response: SubmitConfigSourceResponse>
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicenameconfigssubmit-post-openapi.md
- name: Google Service Management - Get History
  x-api-slug: v1servicesservicenamerollouts-get
  description: |-
    Lists the history of the service configuration rollouts for a managed
    service, from the newest to the oldest.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicenamerollouts-get-openapi.md
- name: Google Service Management - Create new Service Configuration
  x-api-slug: v1servicesservicenamerollouts-post
  description: |-
    Creates a new service configuration rollout. Based on rollout, the
    Google Service Management will roll out the service configurations to
    different backend services. For example, the logging configuration will be
    pushed to Google Cloud Logging.

    Please note that any previous pending and running Rollouts and associated
    Operations will be automatically cancelled so that the latest Rollout will
    not be blocked by previous Rollouts.

    Operation<response: Rollout>
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicenamerollouts-post-openapi.md
- name: Google Service Management - Get Service Configuration
  x-api-slug: v1servicesservicenamerolloutsrolloutid-get
  description: Gets a service configuration rollout.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicenamerolloutsrolloutid-get-openapi.md
- name: Google Service Management - Disable Service
  x-api-slug: v1servicesservicenamedisable-post
  description: |-
    Disables a service for a project, so it can no longer be
    be used for the project. It prevents accidental usage that may cause
    unexpected billing charges or security leaks.

    Operation<response: DisableServiceResponse>
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicenamedisable-post-openapi.md
- name: Google Service Management - Enable Service
  x-api-slug: v1servicesservicenameenable-post
  description: |-
    Enables a service for a project, so it can be used
    for the project. See
    [Cloud Auth Guide](https://cloud.google.com/docs/authentication) for
    more information.

    Operation<response: EnableServiceResponse>
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicenameenable-post-openapi.md
- name: Google Service Management - Undelete Service
  x-api-slug: v1servicesservicenameundelete-post
  description: |-
    Revives a previously deleted managed service. The method restores the
    service using the configuration at the time the service was deleted.
    The target service must exist and must have been deleted within the
    last 30 days.

    Operation<response: UndeleteServiceResponse>
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesservicenameundelete-post-openapi.md
- name: Google Service Management - Generate Configuration Report
  x-api-slug: v1servicesgenerateconfigreport-post
  description: |-
    Generates and returns a report (errors, warnings and changes from
    existing configurations) associated with
    GenerateConfigReportRequest.new_value

    If GenerateConfigReportRequest.old_value is specified,
    GenerateConfigReportRequest will contain a single ChangeReport based on the
    comparison between GenerateConfigReportRequest.new_value and
    GenerateConfigReportRequest.old_value.
    If GenerateConfigReportRequest.old_value is not specified, this method
    will compare GenerateConfigReportRequest.new_value with the last pushed
    service configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1servicesgenerateconfigreport-post-openapi.md
- name: Google Service Management - Get Service State
  x-api-slug: v1name-get
  description: |-
    Gets the latest state of a long-running operation.  Clients can use this
    method to poll the operation result at intervals as recommended by the API
    service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1name-get-openapi.md
- name: Google Service Management - Get IAM Policy
  x-api-slug: v1resourcegetiampolicy-post
  description: |-
    Gets the access control policy for a resource.
    Returns an empty policy if the resource exists and does not have a policy
    set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1resourcegetiampolicy-post-openapi.md
- name: Google Service Management - Set IAM Policy
  x-api-slug: v1resourcesetiampolicy-post
  description: |-
    Sets the access control policy on the specified resource. Replaces any
    existing policy.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1resourcesetiampolicy-post-openapi.md
- name: Google Service Management - Test Permissions
  x-api-slug: v1resourcetestiampermissions-post
  description: |-
    Returns permissions that a caller has on the specified resource.
    If the resource does not exist, this will return an empty set of
    permissions, not a NOT_FOUND error.

    Note: This operation is designed to be used for building permission-aware
    UIs and command-line tools, not for authorization checking. This operation
    may "fail open" without warning.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-service-management/master/_listings/google-service-management/v1resourcetestiampermissions-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.service.control.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.service.management.stack.network
- type: x-change-log
  url: https://cloud.google.com/service-management/release-notes
- type: x-code
  url: https://cloud.google.com/service-management/libraries
- type: x-command-line-interface
  url: https://cloud.google.com/sdk/gcloud/reference/beta/service-management/
- type: x-rate-limits
  url: https://cloud.google.com/service-management/quota
- type: x-support
  url: https://cloud.google.com/service-management/support
- type: x-website
  url: https://cloud.google.com/service-management/overview
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---